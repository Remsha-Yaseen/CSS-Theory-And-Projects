# CSS Animation Guide

## 1. CSS Animation Basics

### Definition
**CSS animations** Allow you to create dynamic, visually engaging effects on web pages without the need for JavaScript or complex programming. They provide a structural way to smoothly transition elements between different style declarations over a specified duration.

### The `@keyframes` Rule
The `@keyframes` rule defines the individual stages, milestones, and styles of a CSS animation. It specifies exactly what styles the targeted element should inherit at various percentage points or states (like `from` and `to`) during the animation timeline.

HTML Structure

```
<link rel="stylesheet" href="styles.css">

<div class="box">Slide</div>
```

```
.box {
  width: 120px;
  padding: 10px;
  background: #0077ff;
  color: white;
  animation: slide-in 1s ease-in-out;
}

@keyframes slide-in {
  from {
    transform: translateX(-100%);
  }
  to {
    transform: translateX(0);
  }
}
```



## 2. The Animation Properties

The CSS `animation` property is a powerful shorthand property used to apply animations to elements. It consolidates the following sub-properties into a single line of code:

* **`animation-name`**: Specifies the precise name of the `@keyframes` rule that the element should use.
* **`animation-duration`**: Sets the total length of time (e.g., in seconds `s` or milliseconds `ms`) that the animation takes to complete one full cycle.
* **`animation-timing-function`**: Defines the acceleration curve of the animation, dictating how it progresses over time (such as `ease`, `linear`, or `ease-in-out`).
* **`animation-delay`**: Specifies a programmatic waiting period before the animation officially begins playing.
* **`animation-iteration-count`**: Sets the total number of times the animation sequence should repeat (can be a specific number or `infinite`).
* **`animation-direction`**: Determines whether the animation sequence plays in the normal forward direction, in `reverse`, or switches directions each cycle using `alternate`.
* **`animation-fill-mode`**: Specifies how the targeted element should retain or apply styles before and after the animation runs (such as `forwards`, `backwards`, or `both`).
* **`animation-play-state`**: Allows you to dynamically `pause` and `resume` the execution of an animation timeline.

---

## 3. Accessibility & User Experience

### The `prefers-reduced-motion` Media Query
One of the primary accessibility concerns with web animations is that sudden or extensive movement can cause severe physical discomfort or harm to some users. Individuals with vestibular disorders, inner ear complications, or high motion sensitivity may experience sudden dizziness, nausea, or intense headaches when exposed to certain motion effects on a screen.

The `@media (prefers-reduced-motion)` media query allows frontend developers to detect if a user has requested minimal or minimized motion settings at their operating system level, allowing the website to strip away triggering animations seamlessly.

### Interactive Element Example

#### HTML Structure
```html
<link rel="stylesheet" href="styles.css">

<button class="animated-element">Hover me</button>
```


#### Accessible CSS Transitions Implementation

```
.animated-element {
  padding: 10px 16px;
  transition: transform 0.3s ease-in-out;
}

.animated-element:hover {
  transform: translateX(20px);
}

/* Accessible fallback for motion-sensitive users */
@media (prefers-reduced-motion: reduce) {
  .animated-element {
    transition: none;
  }
}
```
