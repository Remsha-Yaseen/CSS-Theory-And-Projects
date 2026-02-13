# 🧠 Introduction to CSS

**CSS** stands for **Cascading Style Sheets**. While HTML provides the semantic structure (headers, paragraphs, lists), CSS provides the presentation (colors, layout, fonts).

**The Transformation:** Without CSS, a browser renders HTML in a vertical, black-and-white list. CSS allows us to move elements, add depth, and create branding.

Here is the professional **boilerplate** for CSS3 that you can use in your projects:

<pre>
  
/* 1. THE MODERN RESET */
*, *::before, *::after {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

  
/* 2. ROOT VARIABLES (Design Tokens) */
:root {
    --primary-color: #3498db;
    --secondary-color: #2ecc71;
    --text-color: #333333;
    --bg-color: #ffffff;
    --font-main: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}


/* 3. BASE STYLES */
html {
    scroll-behavior: smooth;
}

body {
    font-family: var(--font-main);
    line-height: 1.6;
    color: var(--text-color);
    background-color: var(--bg-color);
    min-height: 100vh;
    -webkit-font-smoothing: antialiased;
}

  
/* 4. MEDIA ELEMENTS */
img, picture, video, canvas, svg {
    display: block;
    max-width: 100%;
    height: auto;
}
  

/* 5. TYPOGRAPHY HELPERS */
h1, h2, h3, h4, h5, h6 {
    overflow-wrap: break-word;
    line-height: 1.2;
}

  
/* 6. ACCESSIBILITY */
@media (prefers-reduced-motion: reduce) {
    * {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
        scroll-behavior: auto !important;
    }
}

  
</pre>
