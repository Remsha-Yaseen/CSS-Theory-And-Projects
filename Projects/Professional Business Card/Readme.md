# 📋 Overview
This lab focused on creating a clean, centered UI component with a fixed width. The primary goal was to practice container constraints, image responsiveness, and text alignment.

----

## 🚀 Key Techniques Applied

### 1. The Fixed-Width Container
Unlike the Cafe Menu which used a percentage (80%), this project uses a fixed 300px width. This ensures the business card maintains its "card" shape regardless of the screen size.

<pre>
  .business-card {
  width: 300px;
  background-color: white;
  padding: 20px;
  margin: 100px auto; /* Short-hand for centering and top spacing */
  text-align: center;
}
</pre>

### 2. Image Responsiveness
To ensure the profile picture doesn't overflow the 300px card, I implemented a simple but effective fluid image rule. This ensures that if the container ever shrinks, the image stays within the bounds.

<pre>.profile-image {
  max-width: 100%; /* Image will never be wider than its parent */
  height: auto;
}
</pre>

### 3. Typography & Spacing
I used the **Box Model** to tighten the vertical rhythm of the contact information. By default, browsers add large margins to paragraphs; I reduced these to create a professional, compact look.

<pre>
  p {
  margin-top: 5px;
  margin-bottom: 5px;
}
</pre>

### 4. Visual Separation
I used `<hr>` tags combined with standard borders to create logical sections between the bio, contact info, and social links, keeping the information digestible.


### 🧠 What I Learned
**Centering Logic:** Re-enforced that `margin: auto` requires a defined `width` to work.

**Component Thinking:** Learning to build a standalone "card" that can be moved anywhere on a webpage.

**Simplification:** Using `text-decoration:` none to remove default underlines from links for a cleaner UI.
