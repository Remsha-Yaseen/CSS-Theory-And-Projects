# 🔗 CSS Combinators: Mastering Relationships
In CSS, a combinator is something that explains the relationship between selectors. It allows you to be much more specific than just using a class or an ID.

-----

### 1. Descendant Selector (Space)
The most common combinator. It targets any element that is nested inside another, no matter how deep it is.

* **Syntax:** A B (Selector A, space, Selector B)

* **Example:** Styles all <p> elements inside a <div>.

<pre>
div p {
  color: blue;
}
</pre>

**Visual Rule:** If the <p> is a child, grandchild, or great-grandchild, it will turn blue.


### 2. Child Selector (>)
The child selector targets only elements that are immediate children of a parent. It does not go deeper into the family tree.

Syntax: A > B

Example: Styles <p> only if it is directly inside the <div>.

