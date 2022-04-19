# Bootstrap

## What is Bootstrap?
```
A Front-End library
```
```html
<button class="btn btn-primary">Hello World</button>
<button class="btn btn-dark">Hello World</button>
<button class="btn btn-lg btn-outline-dark">Hello World</button>
```
[Bootstrap](https://getbootstrap.com/docs/5.1/getting-started/introduction/) \
[Navbar](https://getbootstrap.com/docs/5.1/components/navbar/) \
[Examples](https://getbootstrap.com/docs/5.1/examples/)

## Installing bootstrap
```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">

<link href="./css/bootstrap.css" rel="stylesheet">
```
[CDN](https://www.akamai.com/es/our-thinking/cdn/what-is-a-cdn)

## Web Design 101 Wireframing
[Wireframing](https://www.lucidchart.com/pages/es/que-es-un-wireframe-para-un-sitio-web) \
[Mockup](https://moqups.com/es/)

## Bootstrap navigation bar
```
ml-auto => ms-auto

mr-auto => me-auto

Practice:
Create <nav> <ul> <li>
Add class navbar-nav nav-item
Make contact a link with nav-link
Add two more links
Make horizontal with navbar-expand-lg
Change background with bg-light
Change style with navbar-light
Create logo with navbar-brand
Creacte a space between links and brand(logo) with margin
Add toggler

Dropdown link
Affect the position of the navbar by changing to Fixed top
```
```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <a class="navbar-brand" href="">tindog</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav ms-auto">
        <li class="nav-item">
            <a class="nav-link" href="">Contact</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">Pricing</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">Download</a>
        </li>
    </ul>
    </div>
</nav>
```
[nav Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav) \
[Navbar](https://getbootstrap.com/docs/5.1/components/navbar/) \
[Buttons](https://getbootstrap.com/docs/5.1/components/buttons/) \
[Spacing](https://getbootstrap.com/docs/5.1/utilities/spacing/)

## Bootstrap grid layout system
```
Create a row div
Create a col div has much has you want
Challenge:
Create two non responsive colums in a row
Create two non responsive colums that are half of the width
Create four responsive colums: large 4, ipad 3, phone 2
Create six responsive colums: large 6, ipad 4, phone 1
```
[Grid](https://getbootstrap.com/docs/5.1/layout/grid/) \
[Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#flexbox-background)

## Containers
```
The container div can contain other div's, buttons, tables, etc, and its automatically responsive.
The fluid container take up 100% of the width.
Obserbation: Inspect the diferent values of the width of the container div, look for @media (max-width) on styles.
```
```html
<div class="container" style="background-color:red">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
</div>
<div class="container-fluid" style="background-color:yellow">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
</div>
```
[Containers](https://getbootstrap.com/docs/5.1/layout/containers/)

## Buttons & Fonts
```html
      <button type="button" class="btn btn-dark btn-lg">Download</button>
      <button type="button" class="btn btn-outline-light btn-lg">Download</button>
```
```
Fontawesome CDN
<script defer src="https://use.fontawesome.com/releases/v5.0.7/js/all.js"></script>
or
<script src="https://kit.fontawesome.com/1c9ad4b785.js" crossorigin="anonymous"></script>
or
<script defer src="https://use.fontawesome.com/releases/v6.1.1/js/all.js"></script>
```
[Buttons](https://getbootstrap.com/docs/5.1/components/buttons/)

## Styling ou website challenge
```
Recap Navbar, buttons, containers, grids
Play with the buttons margin padding
```
[CSS transform property](https://www.w3schools.com/cssref/css3_pr_transform.asp) \
[transform-function](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function) \
[rotate()](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/rotate)

## The Bootstrap Carousel
```
1.-Copy the first example, select carousel-item and give a 500px height and an inline style background color to all 3 item
2.-Put controls buttons to change the slide

Observations:
In class="carousel slide" the slide keywork make the slide efect
See the difference between the slides only and with controls

Exercices:
Change the speed, hover and ride
Try change the <button> for an <a> or <h1>, if you cant try adding "role="button"

Recap:
id="example-target-id": Is the target of data-bs-target="#example-target-id"
data-bs-ride="false": Autoplays the carousel after the user manually cycles the first item
class="carousel slide": The div is gonna be a carousel and the "slide" gives animation from right to left or left to right
carousel-inne: Contain the content of carousel items
carousel-item active: This is the first slide is marked with "active" class and inside this div we can put anything

carousel-contro-prev: Left button
data-bs-target: This is where we put the id of the carousel
data-bs-slide="prev": The direction of the animation
class="carousel-control-next-icon": This is the button icon
aria-hidden="true": This is for visually impaired person and the screen reader doesn't read the button

```
```html
<div id="example-target-id" class="carousel slide" data-bs-ride="false">
  <div class="carousel-inner">
    <div class="carousel-item active" style="background-color:red">
      <img src="..." class="d-block w-100" alt="First item">
    </div>
    <div class="carousel-item" style="background-color:yellow">
      <img src="..." class="d-block w-100" alt="Second item">
    </div>
    <div class="carousel-item" style="background-color:blue">
      <img src="..." class="d-block w-100" alt="Third item">
    </div>
  </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#example-target-id" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#example-target-id" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
```
```css
.carousel-item {
    height:500px;
}
```
[Carousel](https://getbootstrap.com/docs/5.1/components/carousel/)

## Bootstrap cards
```
Bootstrap cards provides a container (look first "Example")

Difference between Bootstrap 4 and 5:
Bootstrap 4: card-deck = Bootstrap 5: card-group
Bootstrap 4: btn-block = Bootstrap 5: w-100 (or use) <div class="d-grid gap-2"> (Block buttons)

For Bootstrap card-deck use the Bootstrap 5 grid system

Challenge: Create a card from scratch with header, a body, and a footer

Challenge: How can you make the third card become 100% at the ipad width, basically medium and below, but keep
the other two only 50%, but only when you get onto the full mobile size do you make all three 100%

Challenge: Make the buttons match the Bootstrap example

Activity: First copy and paste the card "pricing example" in to codeply, next change the "sign up free" button to outline-dark
```
```
Bootstrap card containers have a header, body and footer if you like, here's a solution for the first challenge
```
```html
<div class="card">
    <div class="card-header">
        Card Header
    </div>
    <div class="card-body">
        Card Body
    </div>
</div>
```
```
Solution to the second challenge
```
```html
<div class="row">
    <div class="col-lg-4 col-md-6" style="background-color:yellow; border:1px solid;">
        col
    </div>
    <div class="col-lg-4 col-md-6" style="background-color:yellow; border:1px solid;">
        col
        </div>
    <div class="col-lg-4" style="background-color:yellow; border:1px solid;">
        col
    </div>
</div>
```
[Cards](https://getbootstrap.com/docs/5.1/components/card/) \
[Pricing example](https://getbootstrap.com/docs/5.1/examples/pricing/) \
[Buttons](https://getbootstrap.com/docs/5.0/components/buttons/)
