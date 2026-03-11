# 🚀 CSS Flexbox Technical Review

A comprehensive guide to the one-dimensional layout model for arranging elements in rows or columns.

----


## 1. The Flex Model
Every Flexbox layout consists of a **Flex Container** (parent) and **Flex Items** (children). Layouts are calculated based on two axes:

* **Main Axis**: The primary axis along which items are laid out (defined by `flex-direction`).
* **Cross Axis**: The axis perpendicular to the main axis.



---

## 2. Container Properties

### **Direction & Flow**
| Property | Values | Description |
| :--- | :--- | :--- |
| `flex-direction` | `row`, `row-reverse`, `column`, `column-reverse` | Sets the direction of the main axis. |
| `flex-wrap` | `nowrap`, `wrap`, `wrap-reverse` | Determines if items wrap to new lines. |
| `flex-flow` | `[direction] [wrap]` | Shorthand for both direction and wrap. |



---

## 3. Alignment Logic

### **justify-content (Main Axis)**
Aligns items along the primary direction of the container.
* `flex-start`: Items packed at the start.
* `flex-end`: Items packed at the end.
* `center`: Items centered.
* `space-between`: Items distributed evenly; first at start, last at end.
* `space-around`: Equal space around items; edges have half-size gaps.
* `space-evenly`: All gaps (including edges) are equal.



### **align-items (Cross Axis)**
Aligns items along the perpendicular axis.
* `stretch`: (Default) Items fill the container height/width.
* `flex-start`: Items align to the start of the cross axis.
* `flex-end`: Items align to the end of the cross axis.
* `center`: Items centered along the cross axis.



---

## 4. Key Takeaways
1. **One-Dimensional**: Flexbox handles layout in one direction at a time.
2. **Axis Flipping**: If `flex-direction` is `column`, `justify-content` controls vertical alignment.
3. **Implicit Sizing**: Flexbox allows items to adapt their size to fill available space or shrink to prevent overflow.
