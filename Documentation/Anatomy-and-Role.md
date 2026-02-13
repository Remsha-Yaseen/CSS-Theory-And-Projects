# 🏗️ The Basic Anatomy of a CSS Rule

To transform an element, you must write a Rule Set. Every rule follows a specific syntax:

<pre>
selector {
  property: value;
} 
</pre>


**Selector:** Points to the HTML element you want to style `(e.g., h1, p, or .class-name).`

**Declaration Block:** Everything inside the curly braces `{}.`

**Property:** The specific attribute you want to change `(e.g., background-color).`

**Value:** The setting applied to that property `(e.g., blue).`

----

## The Meta Viewport Element:

Before styling, we must ensure the browser knows how to scale the page on different devices. This is handled in the HTML `<head>:`
<pre>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
</pre>

* **Why it matters:** It ensures your CSS transformations look correct on mobile. Without it, mobile browsers might "shrink" your desktop design to fit the screen, making it unreadable.
