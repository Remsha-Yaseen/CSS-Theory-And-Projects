# Book Inventory Dashboard

A precise, clean front-end component demonstrating advanced **CSS Attribute Selectors**, structural pseudo-classes (`:nth-of-type`), and color-coded status tracking for a personal reading log.

---

## 🚀 Features

* **Dynamic Row Styling:** Rows automatically shift colors based on the book's reading status (`Read`, `In Progress`, `To Read`).
* **Visual Rating System:** CSS-only star/circle rating badges that fill dynamically based on element classes.
* **Pure CSS Logic:** Uses zero JavaScript; all conditional component styles are handled through semantic attributes and relational selectors.

---

## 🛠️ Key CSS Concepts Demonstrated

### 1. Attribute Matching Patterns
Instead of relying solely on class naming conventions, this project utilizes attribute queries:
* `[class="value"]` — **Exact Match:** Targets components matching a highly specific status string (e.g., `tr[class="read"]`).
* `[class^="value"]` — **Prefix Match:** Targets any class starting with a specific term. `span[class^="rate"]` catches styles for any ranking wrapper.
* `[class~="value"]` — **Space-separated Word Match:** Targets sub-classes safely without disrupting the master class configuration (e.g., matching `"one"`, `"two"`, or `"three"` inside `<span class="rate two">`).

### 2. Advanced Structural Pseudo-Classes
To dynamically color the rating circles without hardcoding inline styles on every single child element, advanced indexing is used:
* `span:first-of-type` — Colors exactly the first child node.
* `span:nth-of-type(-n+2)` — Uses an algebraic formula ($an+b$) to match elements conditionally. In this case, it targets indices 1 and 2 to light up a $2/3$ star rating.

---

## 📂 Project Architecture & Syntax

### HTML Structure
The data relies on a semantically standard `<table>` layout utilizing contextual formatting hooks inside table data cells (`<td>`):

```html
<tr class="read">
    <td>Meditations</td>
    <td>Marcus Aurelius</td>
    <td>Philosophy</td>
    <td><span class="status">Read</span></td>
    <td><span class="rate three"><span></span><span></span><span></span></span></td>
</tr>

```

## Applied CSS Rules
The accompanying spreadsheet targets these specific element hierarchies cleanly:

``` html
/* Color-coding data rows via status attributes */
tr[class="read"] {
  background-image: linear-gradient(#e8f5e9, #c8e6c9);
}

/* Linear-algebra selector rules for dynamic multi-circle ratings */
span[class~="two"] span:nth-of-type(-n+2) {
  background-image: linear-gradient(#fdd835, #fbc02d);
}

/* Core circle structures */
span[class^="rate"] > span {
  border: 1px solid #333;
  border-radius: 50%;
  height: 15px;
  width: 15px;
  background-color: #fff;
}

```



### 📊 Mapping Breakdown

| Status Class | Row Theme | Badge Border |
| :--- | :--- | :--- |
| **`read`** | Green Gradient | Dark Green (`#1b5e20`) |
| **`in-progress`** | Blue Gradient | Deep Blue (`#0d47a1`) |
| **`to-read`** | Orange Gradient | Burnt Orange (`#e65100`) |
