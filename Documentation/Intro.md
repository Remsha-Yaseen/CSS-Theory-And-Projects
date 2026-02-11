# 🧠 Introduction to CSS
CSS (Cascading Style Sheets) is the language used to style the visual presentation of a web page. If HTML is the skeleton, CSS is the skin, clothing, and makeup.

---

## 🏗️ The CSS Anatomy
Every CSS rule consists of a Selector and a Declaration Block.

**Selector:** Points to the HTML element you want to style (e.g., h1, .class, #id).

**Property:** The aspect you want to change (e.g., color, font-size).

**Value:** The specific setting you want to apply (e.g., red, 20px).


## 🔌 Ways to Apply CSS
There are **three** ways to add CSS to your HTML document. 

1- Inline CSS
2- Internal CSS
3- External CSS

* External is the industry standard.

**1. Inline CSS**
Applied directly inside the HTML element using the style attribute.

* **Usage:** 

```
<h1 style="color: blue;">Hello World</h1>
```

* **Verdict:** ❌ Avoid. Hard to maintain and messy.

**2. Internal CSS**
Defined within a <style> tag inside the <head> section of an HTML file.

* **Usage:**

```
<style>
  p { color: green; }
</style>
```

* **Verdict:** ⚠️ Okay for small, single-page tests.

**3. External CSS (The Professional Way)**
Linked via a separate .css file using the <link> tag. This is how we build modern websites.

*  **Usage:**

```
 <link rel="stylesheet" href="style.css">
```

* **Verdict:** ✅ Best practice. Keeps code organized and reusable.


## 📝 The CSS Rule Set Example
Here is how a standard rule looks in an external stylesheet:



