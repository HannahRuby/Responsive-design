9
🧩 Responsive Design: MediaQueries

🧩 Responsive Design: MediaQueries
Completion requirements

Responsive Design: Media Queries
Overview
Websites are visited using devices of all shapes and sizes. From a full desktop PC to an Apple watch, phones, folding phones, tablets and more. It's important our websites work as well as possible on as many devices as possible.

We do this using CSS media queries - we "query" the medium the website is being displayed on. We say "If the screen is wider than 800px, put three images side by side".

It allows us to:

Change the layout of the page when the screen is wider or narrower
Change the size of fonts, images and buttons when the screen is wider than a width (using @media (min-width: 800px))
Increase the size of buttons and touch areas for touch screen devices (using @media (pointer: coarse)).
Responding to user needs and accessibility by paying attention to settings like high contrast mode (using @media (prefers-contrast: high))
Class Plan
Demo: Demonstration of media queries, and real world examples of usage in responsive websites (try Smashing Magazine)
Discussion of wireframe: Mobile-first principle - "it is easier to add additional rules for a bigger screen, than to remove a lot of layout rules for a smaller one."
if block elements appear on top of each other by default, what rules might be required to display them side by side?
Workshop: Make your own responsive website with media queries, explore mobile-first design Example Wireframe
Topics
What is a media query?
How to use media queries to change the size of fonts, images and buttons
How to use media queries to change the layout of the page on larger screens
Resources
MDN: Media Queries
Workshop
Setting up the layout
⛳️ In a new project, or one of your existing projects in a new git repo, add a new div with the class container.

<div class="container"></div>
 
⛳️ Select the element in your CSS and apply some basic styles to it.

.container {
  background: #eee;
}
 
🎯 Within the container, add three section elements one after the other with a matching class of box. Add some content or an image to each one.

👀 Notice that by default they stack one on top of the other - this is because sections, divs and many other tags are display: block elements by default. This is ideal for our narrow screen layout.

Adding new rules
👀 Take a look at the simple layout wireframe supplied. To achieve the wide screen layout, we'll need to add some CSS rules to our container, and possibly to our boxes. Flexbox might be the tool for this.

⛳️ Add the media query with the @media keyword, and specifying the min-width: 800px property. These CSS rules will be applied whenever the screen is at least 800px wide, or over. You can also use min-height, max-width and max-height, although we try to avoid the latter and use a small-screen first approach.

@media (min-width: 800px) {
  .container {
    background: plum;
  }
}
 
👀 Confirm that the background colour changes when you resize the browser window above and below 800px.

🎯 Add some more rules inside the media query to change the layout of the boxes to match the wireframe design as closely as possible.

💭 Flexbox is probably a good choice here.

Your answer















