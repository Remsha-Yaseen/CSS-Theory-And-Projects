In CSS, the display property is the most important tool for controlling the layout of a web page. It determines how an element sits on the screen and how it interacts with the elements around it

----

# 🔀 Display Models: Block, Inline, and Inline-Block
Every element in HTML has a default display value. Understanding these values is the key to moving from simple text documents to complex website layouts.


### 1. Block-Level Elements
Block elements are the "bricks" of your layout. By default, they take up the full width available to them.

* **Behavior:** They always start on a new line and push following elements to the next line.

* **Sizing:** You can set a specific width and height.

* **Common Elements:** `<div>`, `<h1>` to `<h6>`, `<p>`, `<ul>`, `<section>`.    

  <pre>

.block-element {
  display: block;
  background-color: lightblue;
  width: 50%; /* Only takes half the screen, but still pushes neighbors away */
  padding: 10px;
}
  </pre>


### 2. Inline Elements
Inline elements are the "thread" within your text. They only take up as much width as their content needs.

* **Behavior:** They sit side-by-side with other inline elements and do not start on a new line.

* **Sizing:** You cannot set a width or height on them. Vertical margin and padding are also ignored or behave strangely.

* **Common Elements:** `<span>`, `<a>`, `<strong>`, `<em>`.


<pre>
.inline-element {
  display: inline;
  color: red;
  /* width: 200px;  <-- This would be ignored */
}
</pre>



