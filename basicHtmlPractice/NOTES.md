
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