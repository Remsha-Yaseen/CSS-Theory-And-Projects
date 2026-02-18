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
