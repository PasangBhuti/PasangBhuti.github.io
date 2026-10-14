
#Reflection 
1. Explain the difference between flex-direction: row and flex-direction: column.

2. Why is it important to use relative units (like %, vh, or rem) instead of fixed pixels (px) for
responsive design?
3. AI Attribution: List the prompt you used if you consulted GenAI. Identify one specific
piece of CSS code the AI provided that you had to modify to make it work for your layout.

# Homework 2 Reflection

## 1. `flex-direction: row` vs. `flex-direction: column`

`flex-direction: row` (the default) lays flex items out horizontally, side by side from left to right. `flex-direction: column` stacks them vertically from top to bottom. The direction also changes how alignment works: with `row`, `justify-content` spaces items horizontally and `align-items` aligns them vertically, and with `column` the two swap roles.

On my site, the navigation links use `row` on desktop so they sit in a line on the right side of the navbar. In my mobile media query (`max-width: 768px`), I switch the nav to `column` so the links stack vertically.

## 2. Why use relative units instead of fixed pixels?

Relative units such as `%`, `rem`, `vh` and `fr` scale with the container, the root font size or the screen size, so the layout adapts to different devices. Fixed `px` values stay the same size no matter what, so a box that is 900px wide would overflow on a 375px phone screen. Using `rem` for text also respects a user's browser font-size settings, which helps accessibility. On my site, the grid uses `1fr` columns and the images use `width: 100%`, so everything resizes smoothly.

## 3. AI Attribution

**Prompts I used:

> modify my answers on 'flex-direction: row' vs 'flex-direction : column' and why use relative units instead of fixed pixels?
> Names of popular fonts that are used on websites?


 CSS code the AI provided when i was figuring out the ratio but i found  `cover` was cropping my pixel-art image and I wanted the whole picture to show.
 > 
/* AI's version */
.card img {
    display: block;
    width: 100%;
    aspect-ratio: 4 / 3;
    object-fit: cover;
}
/* My version */
.card img {
    display: block;
    width: 100%;
    aspect-ratio: 4 / 3;
    object-fit: contain;
    background-color: #ffffff;
}
