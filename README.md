# Project 0

Web Programming with Python and JavaScript

This is a website that pretends to market chili oil. It has links to buy chili oil, pages dedicated 
to the chili oil recipe, and an info page about live Zoom tutorials. The website is good for 
mobile all the way through 4K sized viewports.



## navbar

All pages use the same sticky navbar. The HTML code is written in the header of every .html 
file, and the styling is done on navbar.scss and navbar.css. This navbar was created using 
Bootstrap. Therefore, the links, dropdown, and button were derived from Bootstrap's 
template. When the viewport becomes smaller than a certain number of pixels wide, the links
are replaced with a hamburger dropdown and the logo shrinks significantly. One last thing: 
the buy button as well as the dropdown links lead to Rick Rolls.



## index.html

Styled by index.scss and index.css. This is the home page. All the text and buttons you see
are positioned via absolute positioning. As the viewport gets smaller, the image and the 
buttons scale down automatically. However, the text is manually scaled down in increments 
using @media queries.



## ingredients.html

Styed by ingredients.scss and ingredients.css. This page lists all the ingredients necessary 
for chili oil on a table. Every other row is shaded for ease of reading. In addition, an @media 
query was used to push the contents of the page down when the viewport becomes so small
such that the title of the page would be covered by the logo otherwise.



## procedure.html

This page includes a step-by-step breakdown of how to make chili oil and a list of ingredients
for the user's convenience. They were placed using Bootstrap's grid system. Like with 
ingredients.html, an @media query was used to prevent the title of the page from being 
blocked by the logo on small viewports. Lastly, another @media query was used to make
the ingredients column disappear on mobile-sized viewports.



## class.html

At first glance, class.html seems very similar to index.html, but they are coded in 
completely different ways. First, while index.html's elements were positioned with absolute 
positioning, class.html's elements are coded to be on the center of the page. In addition, 
while index.html's elements are coded with a lot of discrete numbers such as 3px or 40px, 
class.html's elements are coded with a lot of percentages. Thus, class.html scales down 
with the viewport without much use of @media queries.\
This page used Bootstrap's grid system. When the viewport becomes small enough, the 
"join me on Zoom" section will go underneath the class date text.\
And lastly, I should talk about the background. By default, it is an image that scales to the 
height of the viewport. However, to prevenrt exposed empty space, a min-height was given 
to the body of the page and an @media query forces the image to scale the width of wide
viewports.



## template.html

I create for myself a template.html as well as a template.scss to avoid copy and pasting 
repetitive content such as the navbar and SASS variables when creating new pages.
