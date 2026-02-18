# 🎨 Backgrounds and Borders: Visual Surfaces
This module covers the properties used to style the "surface" of an element. We transition from simple solid colors to complex textures using images, gradients, and shaped boundaries.

----

### 1. Background Properties
The `background` property is a shorthand for several individual properties that control the space behind the content.

* `background-color:` Sets a solid color (using names, Hex, RGB, or HSL).

* `background-image:` Places an image or a gradient.

* `background-size:` Controls how the image fits (e.g., `cover` to fill the space or `contain` to show the whole image).

* `background-repeat:` Prevents the image from tiling (using `no-repeat`).

**Linear Gradients**
Gradients are treated as images in CSS. They allow smooth transitions between two or more colors.

<pre>
  .gradient-box {
  /* Syntax: linear-gradient(direction, color1, color2) */
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}
</pre>

----

### 2. Border Properties
Borders define the edge of the Box Model. You can style them as a whole or target specific sides.

* `border-width:` The thickness (e.g., `2px`).

* `border-style:` The type of line (`solid`, `dashed`, `dotted`, `double`).

* `border-color:` The color of the line.

<pre>
  .card {
  border: 2px solid #333; /* Shorthand: width style color */
  border-top: 5px solid blue; /* Specific side targeting */
}
</pre>

----


### 3. Advanced Border Shapes
The `border-radius` property is the most common way to transform a "sharp" box into a "soft" UI component.

* **Rounded Corners:** `border-radius: 10px;`

* **Perfect Circles:** Set a square element (`width` and `height` are equal) to `border-radius: 50%;`.

<pre>
  .avatar {
  width: 100px;
  height: 100px;
  border-radius: 50%; /* Creates a circle */
  border: 3px solid white;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}
</pre>


----



### 📊 Summary Table

| Movie Title | Property | Example Value |
| :--- | :---: | :---: |
| `background-clip` | Determines if background extends under the border. | `padding-box`, `content-box` |
| `background-position` | Moves the image within the container. | `center`, `top right` |
| `border-radius` | Curves the corners of the border box. | `8px`, `50%` |
| `box-shadow` | Adds depth/shadow to the element. | `5px` `5px` `10px` `gray` |
