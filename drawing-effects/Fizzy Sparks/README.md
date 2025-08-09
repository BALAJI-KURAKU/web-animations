# Fizzy Sparks ✨

An interactive particle animation that reacts to your mouse movement, creating vibrant, bouncing sparks with a mirrored reflection effect.  
Built using **HTML5 Canvas**, **JavaScript**, **jQuery**, and **GSAP**.

---

## 🚀 Demo
When you move your mouse over the screen, colorful particles burst from the cursor position, bounce under gravity, and fade away.  
A blurred, mirrored reflection of the sparks adds a glowing aesthetic.

---

## 📂 Project Structure
Fizzy Sparks/
│── index.html     # Main HTML file

│── style.css      # Stylesheet for layout & background

│── script.js      # JavaScript for particle animation logic

---

## 🎨 Features
- **Interactive mouse tracking** – sparks emit from your cursor position.
- **Gravity & bounce physics** – particles fall and bounce off the bottom edge.
- **Dynamic colors** – random hue and brightness for every particle.
- **Smooth animations** – powered by GSAP and `requestAnimationFrame`.
- **Reflection effect** – inverted, blurred particle canvas for a glowing mirror effect.
- **Fully responsive** – canvas resizes dynamically with the window.

---

## 🛠️ Technologies Used
- **HTML5 Canvas API** – drawing and animating particles.
- **JavaScript (ES5)** – logic, particle physics, and rendering.
- **jQuery** – DOM manipulation and event handling.
- **GSAP (TweenMax)** – smooth animations and transformations.
- **imagesLoaded.js** – ensuring animations start after assets are ready.

---

## 📦 Installation & Usage
1. **Clone or download** this repository.
   git clone https://github.com/your-username/fizzy-sparks.git

2. Open index.html in your browser.

3. Move your mouse and watch the magic happen! ✨
---

## ⚙️ How It Works
1. Two canvases (c and c2) are drawn on top of each other.

2. particleFactory() generates particle objects with:

         Random velocity
         
         Random color (HSL)
         
         Radius shrink rate

3. Particles fall under gravity, bounce on impact, and fade away.

4. The second canvas (c2) is scaled vertically (scaleY: -1) and blurred to create a reflection.

5. The animation loop updates at ~60 FPS using setInterval() and canvas redraws.

---
## 📷 Preview
(You can include a screenshot or GIF here)

---
## 💡 Customization
**Particle Size** – Change this.r = 8 in particleFactory().

**Colors** – Adjust the random(30, 60) hue range.

**Gravity** – Change this.gravity = 1 for faster/slower falling.

**Reflection Blur** – Modify filter: 'blur(10px)' for sharper/softer effects.
