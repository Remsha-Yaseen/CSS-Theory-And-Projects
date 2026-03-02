# Realistic CSS Colored Markers

A high-fidelity CSS styling project that transforms simple HTML `div` elements into 3D-rendered markers. This project focuses on mastering the **CSS Box Model**, **depth perception**, and **modern color functions**.

---


## 🚀 Overview
The goal of this project was to move beyond flat design. By layering multiple CSS properties, I simulated light, shadows, and physical materials—like plastic casing and ink—to create a set of realistic markers.



## 🛠️ Key Technical Features

### 1. Depth & Lighting with Gradients
Instead of solid colors, I used **Linear Gradients** to create a "cylindrical" effect. By blending three shades of a color, the markers appear to have a highlight in the center and shadows on the edges.
* **Syntax:** `background: linear-gradient(rgb(min), rgb(mid), rgb(max));`

### 2. The Box Model & Sleeves
To create the marker "sleeve" (the section where the cap meets the body), I utilized the `border-left` property with a `double` style. This adds a realistic ribbed texture without extra HTML.
* **Property:** `border-left: 10px double rgba(0, 0, 0, 0.75);`



### 3. Advanced Color Models
This project demonstrates proficiency in every major CSS color system, specifically focusing on **Alpha channels** for transparency:
* **RGBA:** `rgba(83, 14, 14, 0.8)` — Used for the red marker's depth.
* **Hex8 (Hex with Alpha):** `#3b7e20cc` — Used for the green marker's shadow.
* **HSLA:** `hsla(223, 59%, 31%, 0.8)` — Used for the blue marker's glow.



### 4. Shadow Physics (`box-shadow`)
To make the markers "pop" off the screen, I implemented a centered **glow effect** using the `box-shadow` shorthand property.
* **Blur Radius:** Set to $20px$ to create a soft, diffused light.
* **Offset:** Set to $0$ to ensure the glow radiates evenly, mimicking a front-facing light source.



