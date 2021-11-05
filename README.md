# CSS Camp

# Spec 1
Developer's notes based on next CSS courses:
  > [Modern CSS for Backend Developers](https://laracasts.com/series/modern-css-for-backend-developers)
  Topics:
  - Flexbox
  - Grid with Flex
  - Card design with Flex
  - Card refactor with Tailwind.
  - Sticky Footer with Flex and Tailwind.

# Spec 2
All ideas, tasks and some solutions was created during the watching ["CSS - The Complete Guide 2021 (incl. Flexbox, Grid & Sass)"](https://ibm-learning.udemy.com/course/css-the-complete-guide-incl-flexbox-grid-sass/) by [Maximilian Schwarzmüller, Maximilian Schwarzmüller, Manuel Lorenz](https://academind.com)

> uHost project - build by using
- Different types of selectors
- property and values
- Combinators
- Box model: content, padding, border, margin
- Styling Width and Hight
- box-sizing: content-box, border-box
- display: block, inline, none
- Pseudo classes and Elements: `:hover`, `::first-letter`
- BEM: CSS naming convention
- Color Function: `rgb()`, `rgba()`
- inherit
- `calc()` function to calculate `width`
- `float` to position elements differently, before `flex-box` was introduced. Use with `clear` to not allow another elements take place of floating element, but this is a Bad Approach. `float` great for positioning images and text.
- Using `position` for work with images.

# Notes
- `id=""` selectors have a higher specificity than class selector or pseudo selectors.
- `!important` overwrite specificity, but it's usually bad practice.
- `Document flow` default positioning behavior of html elements.
- `position` property can change `Document flow`. Elements can be remain or excluded from `Document flow`.
- After `position` was added we can move element by using `top, bottom, let, right` with px or % values.
- Positioning Context defines the anchor point for position changes.
- `position: fixed` viewport is Positioning Context. Applicable to block and inline elements.
- `position: absolute` another element is the positioning context, this can either be the HTML element or if we have any ancestors which have the position property applied, this closest ancestor will be positioning context.
- `position: relative` element itself as a positioning context.
- `position: sticky` combination of viewport and another element.
- `z-index` using to change order of elements in depth. To position element above - positive number. To position element below - negative number. Numbers hierarchy dictates the display order. Can be used only with elements that have `position` property with no default value.
- `overflow:hidden` in parent element, will hide/cut child element with changed `position` property.
- Stacking context created when applying `fixed/sticky` or `absolute/relative` in combination with `z-index`. Defines stacking behavior of child elements.

# Tips & Tricks
- Apply `margin: auto` to center group of elements more properly.
- If `html` or any parent element have a `margin` property, for correct `position` display, add `top: 0` and `left: 0`.
