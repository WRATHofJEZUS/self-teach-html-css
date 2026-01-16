
Semantic HTML Cheatsheet...basically

<header> container for content like logos, nav, or site titles ie things that go into header
<nav> defines a section of nav links ie, main menu, login, signup
<main> holds the main content of a page
<article> represents a self-contained piece of content ie blog post, news article
<section> groups related content under a common theme or topic
<aside> contains tangenital or supplementary content ie sidebars or ads
<footer> includes footer info ie copyright notices, contact details, related links

<figure> contains images, diagrams, or code snippets
<figcaption> provides a caption for <figure>
<video> and <audio> embed video/audio with controls, autoplay, loop, and mutted attributes
<time> marks dates or times with "datetime" attribute for machine readability

<data> associates machine-readable values with human-readable content
<meter> and <progress> represent scalar measurements and task progress
<mark> highlights text for reference ie search results
<abbr> defines abbreviations with a "title" attribute for expanded meaning

FlexBox and Grid


---FLEXBOX---
-display: flex || display: inline-flex, enables flex layout on the container
-flex-direction, defines the main axis (row, row-reverse, column, column-reverse)
-flex-wrap, controls wrapping (nowrap, wrap, wrap-reverse)
-flex-flow, shorthand for flex-direction and flex-wrap
-justify-content, aligns items along the main axis
-align-items, aligns items along the cross axis
-align-content, controls spacing between lines when wrapping

-order, changes visual order of items
-flex-grow, defines how much a flex item grows relative to others
-flex-shrink, defines how much a flex item shrinks if necessary
-flex-basis, sets the intial size before space distribution
-flex, shorthand for flex-grow, flex-shrink, flex-basis, ie flex: 1 1 200px
-align-self, overrides align-items for individual items

---GRID---
------container properties------
-display: grid, establishes a grid container
-grid-template-columns: 1fr 2fr;, defines column tracks, proportional fr units, fixed px, or percentages
-grid-template-rows: auto 100px, defines row tracks. Use auto for content-based sizing
-grid-template: "header header" / 1fr 2fr;, shorthand for grid-template-rows, grid-template-columns, grid-template-areas.
-grid-gap: 1rem;, sets gap between rows and columns (use grid-row-gap and grid-column-gap seperatly if needed)
-grid-auto-flow: row;, controls auto-placement direction (default: row, column, or dense for masonry layouts)
-grid-auto-rows: 100px;, sets size of implicitly created rows
-grid-auto-columns: 1fr;, sets size of implicitly created columns
grid-template-areas: "header header" "main aside";, names grid areas for visual layout definition
------child properties------
-grid-column-start: 1;, sets start line for the item in the column axis
-grid-column-end: span 2;, sets end line or spans 2 columns
-grid-column: 1 / span 2;, shorthand for grid-cloumn-start and grid-column-end
-grid-row-start: 2;, sets start line for the items in the row axis
-grid-row-end: 4;, sets the end line or spans 2 rows
-grid-row: 2 / 4;, shorthand for grid-row-start and grid-row-end
-grid-area: header;, assigns a named area (from grid-template-areas) or uses grid-row-start / grid-column-start / grid-row-end / grid-column-end
------alignment and justification------
-justify-items: center;, aligns grid items along the column axis
-align-items: center; aligns grid items along the row axis
-justify-content: center;, aligns the entire grid content along the column axis within the container
-align-content: center;, aligns the grid tracks along the row axis when there's extra space
-justify-self: end;, aligns an individual item along the column axis
-align-self: start;, aligns an individual item along the row axis
------advanced feature------
-minmax(100px, ifr), sets a min and max size for a track (prevents shrinking below 100px)
-repeat(auto-fit, minmax(200px, 1fr)), created responsive grids that adapt to container size
-grid-auto-flow: dense;, fills gaps in grid layouts (for masonry designs)