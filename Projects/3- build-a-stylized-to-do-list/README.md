# 🔗 Lab: Advanced Link Styling & Interactive States
## 📋 Overview
This lab focuses on the behavioral styling of hyperlinks within a nested list structure. The goal was to implement the full lifecycle of a link's state—from unvisited to active—ensuring a highly responsive and accessible user interface.

----

## 🚀 Key Techniques Applied

## 1. The LVHA Ordering Rule
To ensure the CSS styles apply correctly without being overwritten by the **Cascade**, I implemented the link states in the industry-standard order:

* Link (Unvisited)

* Visited (Clicked)

* Hover (Mouse-over)

* Active (Moment of click)

### 2. Accessibility with `:focus`

Unlike the other states that focus on color, the `:focus` state is a critical accessibility feature. It provides a visual "ring" around the link for users navigating via a keyboard.

<pre>
  .sub-item-link:focus {
    outline: 2px solid #ffcc00; /* High contrast outline for accessibility */
}
</pre>


### 3. Nested List Structure
The project uses a nested `ul` (unordered list) hierarchy, allowing for organized task-resource relationships. By using the `.sub-item-link` class, I applied specific styles to sub-links without affecting potential global links elsewhere.

----

### 🔬 CSS Theory in Action

* **Pseudo-classes:** Used `:link`, `:visited`, `:hover`, `:focus`, and `:active` to target elements based on user interaction rather than just their position in the HTML.

* **Inheritance:**  Used a global `a { text-decoration: none; }` to remove underlines from all links, showcasing how parent-level styles flow down to specific classes.

* **Color Theory:**  Implemented distinct colors for "Visited" `(#884488)` vs "Hover" `(#ff4500)` to help the user track their navigation history.

* ---

* ### 🧠 What I Learned

* **User Feedback:** How changing colors on hover makes a website feel "alive" and interactive.

* **Specificity vs. Order:** Why the order of pseudo-classes in the CSS file matters—if `:hover` comes before `:visited`, the hover effect might not show up on links you've already clicked!

* **Clean UI:** How removing `text-decoration` by default can create a more modern, app-like feel.

----

### 📂 Project Files

* `index.html:` Contains the To-Do list with nested resource links.

* `styles.css:` Contains the interactive pseudo-class logic.
