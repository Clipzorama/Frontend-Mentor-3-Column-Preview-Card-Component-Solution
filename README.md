# Frontend-Mentor-3-Column-Preview-Card-Component-Solution
A responsive, 3-column preview card component showcasing different car categories. The project utilizes HTML and CSS, with a focus on flexbox and media queries. Contributions and optimizations are welcome!

## Overview

This project is a 3-column preview card component that adapts to different screen sizes, providing a responsive design experience. The card showcases different car categories with descriptions and a "Learn More" button for each category.

## What I Learned

### CSS !important Rule

In this project, I learned about the !important rule in CSS, which allows for overriding other declarations with higher specificity. This was particularly useful when ensuring that certain styles were applied consistently across different elements, even when more specific rules were in place.

## Flexbox Refresh

I refreshed my understanding of flexbox, especially when it comes to changing the flex-flow property to column. I revisited how the cross-axis and main axis change when you alter the flex direction from its default. This understanding was crucial in designing the responsive layout of the cards.

### Media Queries and Responsiveness

I also worked extensively with the @media decorator to ensure the design is fully responsive. This involved adjusting layouts, dimensions, and font sizes to make the component look great on all devices, from large screens to mobile phones.

## Technologies Used

-- **HTML5**: For structuring the content and ensuring semantic markup.
-- **CSS3**: For styling the component, implementing the responsive design, and managing the layout using flexbox.

### HTML Structure

```html 
<section class="all-content">
    <div class="container">
        <svg width="64" height="40" xmlns="http://www.w3.org/2000/svg"> ... </svg>
        <h2 class="title">SEDANS</h2>
        <p class="car-details">Choose a sedan for its affordability and excellent fuel economy...</p>
        <button id="b1" class="btn">Learn More</button>
    </div>
    <div class="container">
        <svg width="64" height="40" xmlns="http://www.w3.org/2000/svg"> ... </svg>
        <h2 class="title">SUVS</h2>
        <p class="car-details">Take an SUV for its spacious interior, power, and versatility...</p>
        <button id="b2" class="btn">Learn More</button>
    </div>
    <div class="container">
        <svg width="64" height="40" xmlns="http://www.w3.org/2000/svg"> ... </svg>
        <h2 class="title">LUXURY</h2>
        <p class="car-details">Cruise in the best car brands without the bloated prices...</p>
        <button id="b3" class="btn">Learn More</button>
    </div>
</section>
```
### CSS Structure

```css
:root {
    --Bright-orange: hsl(31, 77%, 52%);
    --Dark-cyan: hsl(184, 100%, 22%);
    --Very-dark-cyan: hsl(179, 100%, 13%);
    --Transparent-white: hsla(0, 0%, 100%, 0.75);
    --Very-light-gray: hsl(0, 0%, 95%);
}

.all-content {
    width: 100%;
    height: 95vh;
    display: flex;
    justify-content: center;
    align-items: center;
}

.container {
    width: 300px;
    height: 500px;
    display: flex;
    flex-flow: column wrap;
    align-items: flex-start;
    justify-content: space-around;
    padding: 40px;
}

/* Media query for responsive design */
@media only screen and (max-width: 600px) {
    .all-content {
        flex-direction: column;
        height: auto;
    }

    .container {
        height: 400px !important;
    }
}
```

## Final Thoughts

This project provided an excellent opportunity to solidify my knowledge of responsive design and flexbox. Understanding the intricacies of the !important rule, the behavior of flexbox when changing its direction, and the power of media queries has enhanced my ability to create adaptable and user-friendly web components. I look forward to applying these techniques in future projects.
