# Classified Memo Project

A functional CSS exercise designed to simulate a **redacted government document**. This project focuses on precise box-model manipulation and the use of visual filters to create a "classified" aesthetic.

---

## 📂 Project Features

### **1. Precise Box Modeling**
The core container uses `box-sizing: border-box` to ensure that the `500px` width remains absolute. This allows the `50px` padding and `2px` border to sit inside the defined width without expanding the element's footprint.

### **2. Document Authentication Stamps**
To mimic physical rubber stamps, the `#confidential` and `#top-secret` elements utilize:
* **`display: inline-block`**: Allows the stamps to sit side-by-side.
* **`transform: rotate()`**: Applies slight asymmetrical tilts ($-5^\circ$ and $3^\circ$) to break the digital perfection of the layout.

### **3. Content Redaction**
The project implements the `filter: blur(3px)` property on `.blurred` span elements. This creates a "censored" effect on sensitive information within the paragraph text, simulating a redacted field-agent report.

---

## 🛠️ Technical Objectives Met
* **Main Container**: Fixed 500px width with specific margins and padding.
* **Inline-Block Elements**: Functional use of IDs for specific element styling.
* **CSS Transforms**: Rotation applied to simulate manual stamping.
* **CSS Filters**: Blur effect applied for redaction.
