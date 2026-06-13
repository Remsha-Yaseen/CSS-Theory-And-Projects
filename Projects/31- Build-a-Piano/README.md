# Responsive Piano Project

A CSS-focused project demonstrating the creation of a responsive virtual piano component using absolute positioning, floating elements, and media queries to adapt to various screen sizes.

---

## 🎹 Project Overview

This project builds a stylized piano keyboard entirely with HTML and CSS. It focuses on mastering structural layout techniques, specifically handling complex overlapping elements (like black keys) using CSS pseudo-elements and adaptive responsive design.

---

## 🛠️ Key CSS Concepts Demonstrated

* **Box Sizing:** Implemented `box-sizing: border-box` to ensure padding and borders are included in element dimensions.
* **Absolute & Relative Positioning:** Used to anchor the piano, the logo, and the specific placement of black keys within the keyboard structure.
* **Floating Elements:** Leveraged `float: left` to align the piano keys in a linear sequence.
* **Pseudo-elements:** Used `::after` to create and position black keys onto white keys without needing extra HTML markup.
* **Responsive Media Queries:** Implemented breakpoints to adjust the layout for different devices:
    * **Mobile:** Fixed-width container at `358px`.
    * **Tablet:** Intermediate width of `675px`.
    * **Desktop:** Full-scale layout at `992px`.

---

## 💻 Architecture Summary

### HTML Structure
The piano utilizes a container structure with a grouped `keys` class containing individual `key` `div`s. Black keys are distinguished by the `black--key` modifier class.

### Media Query Breakpoints
The layout adapts using three distinct tiers:

| Breakpoint | Piano Width | Keys Width |
| :--- | :--- | :--- |
| **Mobile (`<= 768px`)** | 358px | 318px |
| **Tablet (`769px` - `1199px`)** | 675px | 633px |
| **Desktop (`> 1199px`)** | 992px | 949px |

---

## 🚀 How to Run
1. Clone this repository to your local machine.
2. Open `index.html` in your preferred web browser to view the piano.
3. Resize your browser window to trigger the responsive layout changes.
