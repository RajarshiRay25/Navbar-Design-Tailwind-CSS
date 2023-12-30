# Navbar-Design-Tailwind-CSS
Certainly! Here's the full Markdown formatted code with comments and explanations for GitHub:

```markdown
# Navbar Design with Tailwind CSS

This repository contains code for a responsive and visually appealing navigation bar designed using Tailwind CSS.

## Table of Contents

1. [Body Classes](#body-classes)
2. [Header Classes](#header-classes)
3. [Nav Classes](#nav-classes)
4. [UL Classes](#ul-classes)
5. [LI Classes](#li-classes)
6. [Button Classes](#button-classes)
7. [Ion-Icon Classes](#ion-icon-classes)

## 1. Body Classes

```html
<body class="font-[Poppins] bg-gradient-to-t from-[#fbc2eb] to- [#a6c1ee] h-screen">
```

- `font-[Poppins]`: Sets the font family to Poppins.
- `bg-gradient-to-t from-[#fbc2eb] to- [#a6c1ee]`: Applies a gradient background from #fbc2eb to #a6c1ee from top to bottom.
- `h-screen`: Sets the height of the body to 100% of the viewport height.

## 2. Header Classes

```html
<header class="bg-white">
```

- `bg-white`: Sets the background color of the header to white.

## 3. Nav Classes

```html
<nav class="flex items-center justify-between w-[92%] mx-auto">
```

- `flex items-center justify-between w-[92%] mx-auto`: Creates a flex container with space between items, 92% width, and centered horizontally.

```html
<div class="nav-links duration-500 absolute md:static md:min-h-fit md:w-auto bg-white min-h-[60vh] left-0 top-[-100%] w-full flex md:items-center md:gap-[4vw] gap-8 px-5">
```

- `absolute`: Positions the element absolutely within its containing element.
- `md:static`: Removes absolute positioning on medium and larger screens.
- `md:min-h-fit`: Sets the minimum height to fit its content on medium and larger screens.
- `md:w-auto`: Sets the width to auto on medium and larger screens.
- `bg-white`: Sets the background color to white.
- `min-h-[60vh]`: Sets the minimum height to 60% of the viewport height.
- `left-0`: Aligns the left edge of the element to the left of its containing element.
- `top-[-100%]`: Positions the top edge 100% above the top edge of its containing element.
- `w-full`: Sets the width to 100%.
- `flex md:items-center md:gap-[4vw] gap-8 px-5`: Creates a flex container with specific gap and padding values on medium and larger screens.

## 4. UL Classes

```html
<ul class="flex md:flex-row flex-col items-center gap-[4vw]">
```

- `flex md:flex-row flex-col items-center gap-[4vw]`: Creates a flex container with row layout on medium and larger screens and column layout on smaller screens, aligning items in the center, and applying a specific gap between items.

## 5. LI Classes

```html
<li>
    <a class="hover:text-gray-500" href="">Products</a>
</li>
```

- `hover:text-gray-500`: Changes text color to gray (#808080) on hover.

## 6. Button Classes

```html
<button class="bg-[#a6c1ee] text-white px-5 py-2 rounded-full hover:bg-[#87acec]">Sign In</button>
```

- `bg-[#a6c1ee]`: Sets the background color to #a6c1ee.
- `text-white`: Sets the text color to white.
- `px-5 py-2`: Sets padding on the x and y axes.
- `rounded-full`: Rounds the corners to make a circular shape.
- `hover:bg-[#87acec]`: Changes the background color on hover.

## 7. Ion-Icon Classes

```html
<ion-icon onclick="onToggleFunction(this)" name="menu-outline" class="text-3xl cursor-pointer md:hidden"></ion-icon>
```

- `text-3xl`: Sets the text size to 3xl.
- `cursor-pointer`: Changes the cursor to a pointer on hover.
- `md:hidden`: Hides the element on medium and larger screens.

```html
<script>
    const nav_links = document.querySelector('.nav-links')
    function onToggleFunction(e){
        e.name = e.name === 'close' ? 'menu' : 'close'
        nav_links.classList.toggle("top-[10%]")
    }
</script>
```

- **JavaScript Function:** Toggles the visibility of the navigation links and changes the ion-icon between 'menu' and 'close' based on user interaction.

---
