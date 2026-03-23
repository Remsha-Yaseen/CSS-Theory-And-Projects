
# CSS Layout and Positioning Reference

A comprehensive guide to understanding document flow, floats, and the various positioning states in CSS.

---

## 1. Working With Floats
**Definition:** Floats remove an element from its normal document flow and position it on the left or right side of its container. Surrounding content (like text) will wrap around the floated element.

* **Properties:** `float: left;`, `float: right;`
* **Clearing Floats:** The `clear` property (e.g., `clear: both;`) is used to move an element below floated content to prevent unwanted overlapping or container collapsing.
* **Clearfix Hack:** A CSS technique used to ensure a parent container maintains its height when it only contains floated children.

---

## 2. Static and Relative Positioning

### Static Positioning
* **The Default:** This is the natural flow of the document. 
* **Behavior:** Elements are rendered from top-to-bottom and left-to-right as they appear in the HTML source.

### Relative Positioning
* **The Offset:** Elements stay within the normal document flow, but can be moved using `top`, `bottom`, `left`, and `right`.
* **Stacking:** It is often used to allow elements to overlap others or to act as a "reference" for absolutely positioned children.

---

## 3. Advanced Positioning Techniques

### Absolute Positioning
* **Independent Behavior:** Removes the element entirely from the normal document flow.
* **Context:** It is positioned relative to its nearest **positioned** ancestor (any ancestor with a position other than `static`).

### Fixed Positioning
* **Viewport Relative:** The element is removed from the flow and positioned relative to the browser window.
* **Behavior:** It stays in a fixed location even when the user scrolls, commonly used for navigation bars.

### Sticky Positioning
* **The Hybrid:** Initially behaves like `relative` positioning, but "sticks" to the viewport (behaving like `fixed`) once the user scrolls past a certain point.
* **Use Case:** Ideal for headers that stay at the top of the screen only after you scroll down to them.

---

## 4. Stacking with `z-index`
**Definition:** The `z-index` property controls the vertical stacking order of overlapping elements.

* **Requirement:** Only works on elements that have a `position` value other than `static` (e.g., `relative`, `absolute`, `fixed`, or `sticky`).
* **Logic:** Elements with higher `z-index` values appear on top of elements with lower values.

