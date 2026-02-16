# 🧠 The Cascade, Specificity, and Inheritance
**CSS** stands for **Cascading Style Sheets**. The "Cascade" is the set of rules the browser uses to decide which CSS property value wins when an element is targeted by multiple rules.

----

### 1. The Cascade (The Tie-Breaker)
When two or more CSS rules point to the same element, the browser looks at three factors (in this order) to determine the winner:

**1- Importance:** Rules marked with `!important` win (use sparingly).

**2- Specificity:** The more "specific" a selector is, the more weight it has.

**3- Source Order:** If importance and specificity are equal, the last rule written in the CSS file wins.



### 2. Specificity Hierarchy
Think of specificity as a score. The higher the score, the more powerful the selector.

| Selector Type | Example | Specificity Score |
| :--- | :---: | :---: |
| ID Selector | #header | Very High |
| Class / Pseudo-class | .menu / :hover | Medium |
| Element Selector | h1, p, div | Low |
| Universal Selector | * | Zero |

**Rule of Thumb:** An ID will always beat a Class, and a Class will always beat an Element selector.


### 3. Inheritance
Inheritance is the process by which certain CSS properties are passed down from a parent element to its children.

* **Inherited Properties:** Mostly text-related properties like `color`, `font-family`, and `line-height`.

* **Non-Inherited Properties:** Layout-related properties like `margin`, `padding`, `border`, and `width`.

<pre>
body {
  color: blue; /* Every child of body will now have blue text */
  border: 1px solid black; /* Only the body gets the border; children do NOT inherit it */
}
</pre>


### 4. Forced Inheritance Keywords
You can manually control inheritance using these keywords:

* **inherit:** Forces a child to take the property value from its parent.

* **initial:** Sets the property back to the default browser value.

* **unset:** Resets a property to its inherited value (if it inherits) or its initial value (if it doesn't).

| Concept | Definition | 
| :--- | :---: | 
| Cascade | The logic used to resolve CSS rule conflicts. |
| Specificity | The weight assigned to different types of selectors. | 
| Inheritance | How children gain styles from their parent elements. | 


