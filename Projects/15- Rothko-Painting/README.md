# CSS Rothko Painting

A technical study in **Abstract Expressionism** using modern CSS. This project recreates the soft, vibrating color fields of Mark Rothko by breaking the rigid geometry of the browser's box model.

---

## 🎨 Core Techniques

### **1. Atmospheric Softness**
To move away from sharp digital edges, we used a layering system to create a "glow":
* **`filter: blur()`**: Softens the entire canvas and individual shapes.
* **`box-shadow`**: Matching the shadow color to the background with a specific `spread-radius` to simulate paint bleeding into the fabric.

### **2. Organic Form**
To mimic the human hand, we introduced intentional "errors":
* **Asymmetrical `border-radius`**: Different values for each corner (e.g., `30px 25px 60px 12px`) to warp the rectangles.
* **Micro-Rotations**: Using `transform: rotate()` between -0.6deg and 0.4deg to create a rhythmic "sway."

### **3. The Color Stack**

| Layer      | Hex Code  | Visual Role           |
| :--------- | :-------- | :-------------------- |
| **Canvas** | `#4d0f00` | Deep mahogany base    |
| **Top** | `#efb762` | Golden amber glow     |
| **Middle** | `#8f0401` | Deep crimson heart    |
| **Bottom** | `#b20403` | Vibrant red base      |

---

