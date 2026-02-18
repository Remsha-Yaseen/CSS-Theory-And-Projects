# ☕ Lab: Camper Cafe Menu

## 📋 Overview
This workshop project focuses on creating a multi-section cafe menu. The goal was to practice advanced positioning, typography, and background layering.

## 🚀 Key Techniques Applied

### 1. Advanced Positioning with Inline-Block
To get the "Flavor" and "Price" on the same line, I used `display: inline-block`. By setting specific widths (75% and 25%), I created a clean, aligned list without using tables.
```css
.flavor, .dessert {
  text-align: left;
  width: 75%;
}

.price {
  text-align: right;
  width: 25%;
}


### 2. Centering & The Box Model
I used **margin-left:** auto and **margin-right:** auto to center the **.menu** div. I also used **max-width: 500px** to ensure the menu doesn't get too wide on large desktop screens.

### 3. Interactive Link States (Pseudo-classes)
I followed the LVHA rule (Link, Visited, Hover, Active) to ensure the footer link provides visual feedback to the user.


<pre>
a:hover { color: brown; }
a:active { color: brown; }
</pre>

### 4. Background Layering
I practiced layering by putting a repeating coffee bean image on the body and a solid "burlywood" color on the main container to create a "paper menu" effect.

