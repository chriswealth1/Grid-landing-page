#  - Grid Landing Page

This project is a solution to a **Frontend Mentor** challenge, focusing on building a balanced, clean UI using advanced CSS techniques.

##  Features

* **Balanced Hero Section:** Utilizes **CSS Flexbox** .
* **Responsive 2x2 Grid:** Leverages **CSS Grid** to display a structured 4-card matrix on desktop that collapses seamlessly into a single-column layout on mobile viewports.
* **Interactive Navigation Overlay:** Includes a slide-out hamburger menu panel designed for smooth transitions on smaller screens.
* **Sticky Navigation Bar:** Prompts an active background color change when toggled to maximize visibility.

##  Tech Stack

* **Structure:** HTML5 (Semantic elements like `<main>`, `<section>`, `<article>`, `📄`)
* **Styling:** CSS3 (Flexbox, CSS Grid, Custom Media Queries)
* **Fonts:** Inter via Google Fonts
* **Interactivity:** Vanilla JavaScript (DOM manipulation for menu toggles)

## Combining Flexbox & Grid

Here is a simplified look at how this project uses **Flexbox** to manage the main layout direction and **CSS Grid** to handle the structured multi-column card layout inside it.

```css
/* 1. Outer Layout managed by Flexbox */
.hero .parent {
    display: flex;
    flex-direction: row; /* Aligns text side-by-side with the grid on desktop */
    align-items: center;
}

/* 2. Inner Layout managed by CSS Grid */
.stats-parent {
    display: grid;
       display: grid;
    flex: 50%;
    grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
    grid-auto-rows: minmax(230px,auto);                   
}

/* 3. Mobile Responsiveness */
 @media screen and (max-width:375px) {
        .hero .parent{
        display: flex;
        flex-direction: column;
        align-items: stretch;
         }
    .parent-title , .stats-parent{
        flex:100%;
    }
```


## Contact

* **Your Name** - [chriswealth1](https://github.com)
* **Frontend Mentor Profile:** [@chriswealth1](https://frontendmentor.io)
