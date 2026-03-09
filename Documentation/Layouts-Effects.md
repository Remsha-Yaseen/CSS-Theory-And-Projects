# CSS Layouts and Effects 

This summary covers the essential principles of the CSS box model, positioning, and visual enhancement properties used in modern web development.

---

## 1. The Box Model & Sizing
Every HTML element is treated as a rectangular box consisting of four layers: **Content**, **Padding**, **Border**, and **Margin**.

* **Box-Sizing**:
    * `content-box` (Default): Width and height apply only to the content. Padding and borders are added to the outside, increasing the total size.
    * `border-box`: Width and height include padding and borders. This makes layout calculations much more predictable.
* **Margin Collapse**: Vertical margins (top and bottom) of adjacent elements overlap rather than add together, resulting in a single margin equal to the larger of the two.



## 2. Layout & Overflow Management
* **Overflow**: Controls how content is handled when it is too large for its container.
    * `overflow-x`: Manages horizontal overflow.
    * `overflow-y`: Manages vertical overflow.
* **CSS Reset**: A practice of clearing default browser styles (using tools like `normalize.css`) to ensure a consistent look across different browsers.



## 3. CSS Transform Property
Transforms allow elements to be modified in 2D or 3D space without affecting the surrounding layout flow.
* **`translate()`**: Moves an element from its current position.
* **`scale()`**: Increases or decreases the size of an element.
* **`rotate()`**: Tilts an element by a specified degree (e.g., `45deg`).
* **`skew()`**: Distorts an element along the X or Y axis.



## 4. CSS Filter Property
Filters apply graphical effects to elements, similar to photo editing software.
* **`blur()`**: Applies a Gaussian blur (measured in pixels).
* **Color Adjustments**: Includes `brightness()`, `contrast()`, `grayscale()`, and `sepia()` (measured in percentages).
* **`hue-rotate()`**: Shifts the color of an element around the color wheel (measured in degrees).



---
