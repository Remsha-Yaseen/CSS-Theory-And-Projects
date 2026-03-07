# Feature Selection UI

A modern, accessible **Feature Selection** interface built with semantic HTML and custom-engineered CSS. This project demonstrates the ability to "skin" native browser inputs, replacing default checkboxes with a bespoke, interactive design.

----


## 🚀 Key Features
* **Custom UI Elements:** Completely replaces native browser styling using `appearance: none`.
* **State-Driven Design:** Uses the `:checked` pseudo-class to trigger dynamic style changes.
* **SVG-free Checkmarks:** Leverages the `::after` pseudo-element and Unicode characters for a lightweight footprint.
* **Fully Responsive:** Uses a flexible `feature-card-container` to maintain layout integrity across devices.

## 🛠️ Technical Implementation
* **HTML5:** Utilizes `<label>` wrappers to ensure a large, accessible hit-area for every feature card.
* **CSS3 Specificity:** Implements attribute selectors (`input[type="checkbox"]`) for targeted styling without class-bloat.
* **Visual Polish:** Employs absolute positioning and CSS transforms to achieve pixel-perfect centering of the checkmark icon.

## 🎨 Design Logic
The checkbox transitions from a hollow, bordered state to a solid "active" state when toggled. This provides immediate visual feedback to the user, a core principle of good UX design.



---

### 🖥️ How to Use
1. Clone this repository.
2. Open `index.html` in your favorite web browser.
3. Interact with the feature cards to see the custom CSS state transitions!
