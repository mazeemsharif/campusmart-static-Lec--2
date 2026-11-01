# CampusMart - Responsive CSS Edition

A modern, fully responsive, and accessible frontend for **CampusMart**, a student marketplace where university students can buy and sell second-hand items. 

This repository contains the completed work for **Lecture 2: CSS3 - Box Model, Flexbox, Grid & Responsive Design** (CS554 Advanced Web Technologies). It builds upon the semantic HTML5 structure from Lecture 1 by adding hand-written CSS, without relying on any external frameworks like Bootstrap or Tailwind.

## 🎨 Key CSS Features Implemented

* **Box Model Reset:** Uses `box-sizing: border-box` globally to ensure predictable element sizing and prevent layout breaking.
* **Flexbox Navbar:** A sticky, responsive header using `display: flex` to perfectly align the logo and navigation links.
* **CSS Grid Layouts:** 
  * The **Listing Cards** use `grid-template-columns: repeat(auto-fill, minmax(240px, 1fr))` for a fluid, responsive gallery that adapts to the screen size without media queries.
  * The **Sell Form** uses Grid to stack the Category and Price inputs on mobile, but places them side-by-side on screens ≥ 768px.
* **Dark Mode:** Uses CSS custom properties (variables) inside `:root` and a `@media (prefers-color-scheme: dark)` query. The site automatically switches themes based on the user's operating system preferences.
* **Modern Typography:** Uses `clamp()` on the hero heading to create fluid text that scales smoothly with the viewport width.
* **Accessibility & Focus:** Removes `outline: none` and replaces it with a clear `:focus-visible` ring for keyboard navigators.
* **Container Queries:** Uses `container-type: inline-size` on the grid to adjust the card layout based on the container's width, not just the screen size.

## 📂 Project Structure

```text
campusmart-static/
├── index.html       # Homepage with hero section and responsive card grid
├── sell.html        # Accessible form with HTML5 validation and CSS Grid layout
├── about.html       # Informational page
├── styles.css       # The shared stylesheet containing all CSS rules
└── README.md        # Project documentation
