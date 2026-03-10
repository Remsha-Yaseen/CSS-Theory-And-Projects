# 📸 CSS Flexbox Photo Gallery

A modern, responsive image gallery built to practice **CSS Flexbox** and responsive design principles. This project focuses on creating a clean, uniform grid of images that adapts seamlessly to different viewport sizes while maintaining accessibility.

----

## 🚀 Key Features

* **Fluid Flexbox Grid**: Utilizes `display: flex` and `flex-wrap` to create a layout that flows naturally across mobile, tablet, and desktop.
* **Uniform Image Sizing**: Uses `object-fit: cover` to ensure various images fit into a fixed $350px \times 300px$ container without stretching or squishing.
* **The "Ghost Element" Alignment**: Implements a `::after` pseudo-element to solve common Flexbox alignment issues, ensuring the last row of images stays correctly positioned.
* **Responsive Constraints**: Features a `max-width: 1400px` container with `margin: 0 auto` to prevent the gallery from becoming too wide on large monitors.
* **Accessibility First**: Every image includes descriptive `alt` text for screen readers and SEO optimization.



## 🛠️ Technologies Used

* **HTML5**: Semantic structure and accessible image attributes.
* **CSS3**: Flexbox layout, Pseudo-elements (`::after`), and the Box Model.

## 📂 Project Structure

* `index.html` - Contains the gallery structure and image content.
* `styles.css` - Contains all layout, responsive design, and aesthetic styling rules.



