# Custom Game Settings Panel

A sleek, interactive **Game Settings** interface built with semantic HTML and modern CSS. This project focuses on the art of **checkbox skinning**, replacing default browser inputs with custom-designed, animated elements.

---

## 🚀 Features
* **Fully Custom Checkboxes:** Utilizes `appearance: none` to build checkboxes from scratch.
* **Dynamic Feedback:** Features smooth color transitions and pseudo-element (`::after`) injections for checkmark indicators.
* **Accessible Design:** Labels are wrapped around inputs to provide a large, user-friendly click target.
* **Responsive Layout:** Uses a centered "Settings Card" design with `max-width` and `box-shadow` for a polished, modern look.

## 🛠️ Technologies Used
* **HTML5:** Semantic structure with labels and inputs.
* **CSS3:** Advanced selectors, pseudo-classes (`:checked`), pseudo-elements (`::after`), and transitions.

## 🎨 Key CSS Techniques
To achieve the custom look, the project uses the following logic:
* **Customizing the box:** `appearance: none` removes the browser default.
* **The Checkmark:** `content: "✓"` is injected via `::after` only when the `:checked` state is active.
* **Alignment:** `line-height` and `vertical-align` are used to perfectly center the custom checkmark.



---

### 🖥️ How to Run
1. Clone the repository.
2. Open `index.html` in any modern web browser.
3. Toggle the settings to see the CSS transitions in action!
