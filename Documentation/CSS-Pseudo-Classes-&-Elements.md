# 🎨 CSS Pseudo-Classes & Elements Guide

A comprehensive cheat sheet and implementation of modern CSS selectors for creating interactive and dynamic web interfaces.

---

## 🖱️ User Action
* **`:hover`** – Styles an element when the mouse is over it.
* **`:active`** – Styles an element while it is being clicked.
* **`:focus`** – Styles an element when it gains focus.
* **`:focus-within`** – Styles a container if any child inside it has focus.

## 📝 Form & Input States
* **`:checked`** – Targets selected checkboxes or radio buttons.
* **`:valid` / `:invalid`** – Styles inputs based on HTML validation rules.
* **`:required` / `:optional`** – Styles fields based on the presence of the `required` attribute.
* **`:disabled` / `:enabled`** – Targets elements based on their interactivity.



## 🌳 Tree-Structural
* **`:root`** – Targets the `<html>` element (best for global CSS variables).
* **`:nth-child(n)`** – Selects an element based on its position in the parent.
* **`:first-of-type` / `:last-of-type`** – Selects the first or last occurrence of a tag.
* **`:empty`** – Targets elements that have no children or text.

## ⚙️ Functional & Logical
* **`:is()` / `:where()`** – Handles a list of selectors efficiently (`:where` has 0 specificity).
* **`:not(selector)`** – Excludes specific elements from a style rule.
* **`:has(selector)`** – Styles a parent element if it contains a specific child.



## ✨ Pseudo-elements
* **`::before` / `::after`** – Inserts decorative content via the `content` property.
* **`::marker`** – Styles list bullets or numbers.
* **`::first-letter`** – Styles the very first character of a block of text.

---

## 🛠️ Usage Example
```css
/* Styling a label only when its radio button is checked */
input[type="radio"]:checked + label {
    color: #2ecc71;
    font-weight: bold;
}



