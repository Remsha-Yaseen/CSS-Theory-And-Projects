# 🌐 CSS Accessibility & Responsive Design

This document serves as a reference for maintaining high accessibility standards and implementing responsive CSS features in web projects.

---

## 🛠️ Color Contrast & Diagnostic Tools
Ensuring text is legible is the foundation of accessible design.
* **WebAIM's Color Contrast Checker**: An online tool used to verify that foreground and background colors meet **WCAG** (Web Content Accessibility Guidelines) standards.
* **TPGi Colour Contrast Analyzer**: A desktop application for checking contrast that includes a **Color Blindness Simulator**, allowing developers to see their site through the perspective of users with various vision impairments.

## 🌳 The Accessibility Tree
The **Accessibility Tree** is a specialized version of the DOM (Document Object Model). It contains the objects that assistive technologies, such as screen readers, use to interpret and interact with the content on a webpage.

## 📏 Modern CSS: The `max()` Function
The `max()` function selects the largest value from a comma-separated list of values. 
* **Example**: `width: max(25vw, 250px);`
* **Behavior**: If the viewport is smaller than `1000px`, `25vw` (25% of the viewport) is less than `250px`, so the width stays at **250px**. If the viewport is wider than `1000px`, the width becomes **25vw**.

---

## 🛡️ Best Practices for CSS & Accessibility

### Hiding Content
Choosing the correct method to hide content is critical for screen reader compatibility:
* **`display: none;`**: Completely removes the element from both the visual layout and the **Accessibility Tree**.
* **`visibility: hidden;`**: Hides the element visually and removes it from the **Accessibility Tree**, but the element still occupies physical space in the document flow.
* **`.sr-only` CSS Class**: A standard utility class used to hide content visually while keeping it fully accessible to screen readers.

### Motion Control
To accommodate users with vestibular disorders or motion sensitivity:
* **`scroll-behavior: smooth;`**: Enables fluid scrolling between page anchors.
* **`prefers-reduced-motion`**: A media feature used to detect the user’s system-level preference for reduced animation.

```
@media (prefers-reduced-motion: no-preference) {
  * {
    scroll-behavior: smooth;
  }
}
```


## 🏷️ HTML Attributes for Accessibility

### Hiding with Attributes
* **`aria-hidden="true"`**: Hides an element specifically from assistive technologies (like screen readers) while keeping it visible on the screen. This is best used for decorative elements that do not add meaningful context.
* **`hidden` attribute**: A native HTML attribute supported by most modern browsers. It hides content both visually and from the Accessibility Tree, and can be easily toggled using JavaScript.

### The Placeholder Issue
The `placeholder` attribute should **not** be used as a replacement for the `<label>` element. Using it as a label creates several accessibility barriers:

* **Confusion**: Users often mistake placeholder text for an actual input value, leading them to think the field is already completed.
* **Loss of Context**: Once a user begins typing, the placeholder disappears. This removes the instruction or hint, which can be particularly difficult for users with cognitive or memory-based disabilities.
