# CSS Color Box Palette

A clean, responsive color grid designed to demonstrate proficiency in various **CSS Color Models** and the **Box Model**. This project showcases how to implement colors using Hexadecimal, RGB, HSL, and Named color values within a structured grid layout.

----

## 🚀 Project Objective
The goal of this lab was to build a visually cohesive color palette where each element is styled using a different CSS color declaration method. 

----

## 🛠️ Technical Implementation

### 1. The Color Grid Structure
The project uses a container-child architecture. A parent `div` with the class `.color-grid` acts as the flex-container, housing five individual `.color-box` elements.

### 2. Diversified Color Declarations
To meet the project requirements, each box utilizes a distinct color system:
* **Color 1 (Hex):** `#3498db` — Demonstrates the use of base-16 hexadecimal notation.
* **Color 2 (RGB):** `rgb(46, 204, 113)` — Uses the Red-Green-Blue additive model.
* **Color 3 (Named):** `tomato` — Uses a predefined CSS keyword.
* **Color 4 (HSL):** `hsl(280, 60%, 50%)` — Employs the Hue-Saturation-Lightness model for intuitive color picking.
* **Color 5:** A deep slate finish to complete the palette.



### 3. Styling & Layout
* **Centering:** The `body` uses Flexbox (`justify-content: center` and `align-items: center`) to ensure the palette is perfectly centered on any screen size.
* **Box Model:** Every `.color-box` has a uniform `width` and `height` to maintain visual consistency.
* **Background:** The workspace uses a light gray background (`#f4f4f4`) to allow the vibrant colors of the boxes to stand out.



## ✅ User Stories Fulfilled
- [x] Set `body` background to `#f4f4f4`.
- [x] Created a `.color-grid` container.
- [x] Implemented five `div` elements with class `color-box`.
- [x] Applied specific class names `color1` through `color5`.
- [x] Verified all color systems (Hex, RGB, Word, HSL) are functioning correctly.

## 📝 How to View
1. Clone this repository.
2. Open `index.html` in your browser.

---
Created as part of a CSS Color Systems Deep-Dive.
