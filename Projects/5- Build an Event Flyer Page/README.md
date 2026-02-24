# Event Flyer Project
A responsive web layout designed to demonstrate the effective use of **CSS units** and **dynamic calculations**. This project focuses on moving away from fixed-pixel layouts toward fluid designs that adapt to the user's viewport.

----

### 🚀 Key Features

* **Responsive Body Sizing:** Uses `vw` (Viewport Width) units to ensure the content width scales according to the browser window.

* **Dynamic Height Calculation:** Implements the `calc()` function to ensure the page fills the screen perfectly without unnecessary scrollbars.

* **Fluid Sections:** Uses percentage-based widths for the `main` content and `hr` elements to maintain consistency across devices.

* **Accessible Typography:** Structured using semantic HTML5 (`header`, `main`, `section`) for better screen-reader support.

### 🛠️ Technical Concepts Applied

**1. The `calc()` Function**
I used `calc()` to handle the vertical layout logic. Since the body has a total vertical padding of 100px (50px top + 50px bottom), I calculated the `min-height` as follows:

<pre>
  min-height: calc(100vh - 100px);
</pre>

This ensures the element is exactly as tall as the viewport minus the space taken by padding.

### 2. Viewport Units vs. Percentages

* **vw:** Used on the `body` to define width relative to the entire browser window.

* **%:** Used on `section` elements to define width relative to the `body` container, ensuring internal consistency.

  ### 3. Centering Logic
By combining a relative width with `margin: 0 auto;`, the flyer remains perfectly centered on large screens while remaining flexible on mobile devices.

### 📂 Project Structure

* `index.html`: Contains the semantic structure (Header, Main, Sections).

* `styles.css`: Contains the layout logic and responsive units.
