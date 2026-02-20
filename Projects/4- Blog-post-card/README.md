# 📋 Overview
This project focuses on the visual "polishing" of a web component. It demonstrates how to combine images, typography, and depth effects (like shadows and transitions) to create a card that looks like it belongs on a modern tech blog.

---

## 🚀 Key Techniques Applied

### **1. Rounded Corners & Overflow Control**

To achieve a modern look, I used `border-radius`. A key challenge was ensuring the image also followed the card's curves. By using `overflow: hidden` on the parent container, the image is automatically "clipped" to fit the rounded corners.

<pre>
  .blog-post-card {
    border-radius: 12px;
    overflow: hidden; /* Vital for clipping child images */
}
</pre>


### 2. Adding Depth with Box-Shadow

To make the card "pop" off the page, I used the `box-shadow` property. This creates a sense of hierarchy and elevation.

<pre>
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
</pre>

### 3. Transitions & Interaction
I implemented a `transition` on the "Read More" button. This ensures that when a user hovers over the button, the color change happens smoothly rather than instantly, creating a premium feel.

<pre>
  .read-more {
    transition: background-color 0.3s ease;
}
</pre>

### 4. Centering with Flexbox (Introduction)
For this lab, I used **Flexbox** on the `body` to perfectly center the card both horizontally and vertically on the screen, regardless of the device size.

----


### 🔬 CSS Theory in Action

* **Image Handling:** Using `display: block` and `width: 100%` on the `.post-img` ensures there are no unwanted gaps at the bottom of the image and that it fits the container perfectly.

* **Typography:** Using a combination of `rem` units for font sizes and specific hex codes (`#1e293b`) for better readability and color contrast.

* **The Accent Border:** Using a `border-bottom` on the image serves as a visual "divider" and adds a pop of brand color (Indigo).

---


### 🧠 What I Learned

* **Encapsulation:** How to wrap content in a `.post-content` div to apply uniform padding without affecting the full-width image above it.

* **RGBA Colors:** Using `rgba` for shadows allows for transparency, making the shadow look natural rather than a solid gray block.

* **Mobile-First Thinking:** By setting a `width: 350px` but using a flexible `body`, I've created a component that works well on different viewports.
