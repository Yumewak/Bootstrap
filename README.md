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
[Bootstrap](https://getbootstrap.com/docs/5.1/getting-started/introduction/)
[Navbar](https://getbootstrap.com/docs/5.1/components/navbar/)
[Examples](https://getbootstrap.com/docs/5.1/examples/)

## Installing bootstrap
```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">

<link href="./css/bootstrap.css" rel="stylesheet">
```
[CDN](https://www.akamai.com/es/our-thinking/cdn/what-is-a-cdn)

## Web Design 101 Wireframing
[Wireframing](https://www.lucidchart.com/pages/es/que-es-un-wireframe-para-un-sitio-web)
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
[Grid](https://getbootstrap.com/docs/5.1/layout/grid/)

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

```
