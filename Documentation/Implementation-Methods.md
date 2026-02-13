# 🔌 Ways to Apply CSS

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

<pre>
/* This is a CSS Comment */
p {
  color: #333;            /* Property: Value */
  font-family: Arial;     /* Property: Value */
  text-align: center;     /* Property: Value */
}
</pre>
