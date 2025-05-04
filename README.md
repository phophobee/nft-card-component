# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Links

- Solution URL: [Git Repository](https://github.com/phophobee/nft-card-component)
- Live Site URL: [GitHub Pages](https://phophobee.github.io/nft-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

✅ HTML Learning Points
Semantic HTML Elements

Card Layout Structure
Understand how to build a reusable component (a card) with nested elements like image, title, description, metadata, and author info.

Class Naming and BEM Approach (optional)
Use class names to logically separate styling concerns (e.g., card, creator-info, price-info, etc.).

Accessibility Considerations
Learn the importance of using alt attributes for images and using text content for clarity.

Interactive Elements
Implement hover interactions by wrapping items like titles or usernames in anchor (<a>) tags.

✅ CSS Learning Points
Flexbox Layout
Use display: flex, justify-content, and align-items to align and space elements inside the card cleanly.

Hover States
Use the :hover pseudo-class to create visual feedback when users interact (e.g., changing image overlay, text color).

Transitions and Effects
Learn how to use transition for smooth animations during hover events.

Positioning and Layering
Understand position: absolute/relative, z-index, and overlays (like the eye icon when hovering over the image).

Color and Typography Styling
Practice using font sizes, weights, and color contrasts for visual hierarchy and readability.

Responsive Design
Use @media queries to make your layout adapt gracefully to different screen sizes, especially mobile.

Padding and Margins
Learn how to use spacing utilities to control layout and breathing space within and between components.

Border Radius and Shadows
Use border-radius and box-shadow to create smooth, card-like UI with depth.

Custom Icons and Assets
Use external SVG icons or image assets inside HTML and style them for interaction.

Background Overlays
Learn to use semi-transparent overlays (e.g., dark layer + eye icon on hover) to create depth and interactivity.

```html
<div class="card-image">
  <img
    src="./images/image-equilibrium.jpg"
    alt="Equilibrium"
    class="main-image"
  />
  <div class="overlay">
    <img src="./images/icon-view.svg" alt="View Icon" class="view-icon" />
  </div>
</div>
```

```css
.card-image .overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 255, 247, 0.5);
  opacity: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  transition: opacity 0.3s ease;
}
```

## Author

- Frontend Mentor - [@phophobee](https://www.frontendmentor.io/profile/phophobee)
