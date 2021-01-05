# Responsive Portfolio - Bootstrap & CSS Assignment

![Responsive Porfolio Screenshot](dist/assets/img/screenshot.png)

> <h2 align="center"><a  href="https://kevin-aminzadeh.github.io/02-bootstrap-responsive-portfolio/">Live Demo</a></h2>

## Table of Contents

- [Overview](#overview)
- [Technologies Used](#technologies-used)
- [Requirements](#requirements)
- [Approach](#approach)
- [License](#license)

## Overview

This project is a simple responsive portfolio site built using the Bootstrap framework.

The aim of this exercise is to showcase the benefits of utilizing a CSS framework for building smaller projects and rapid prototyping, as well as to reinforce basic CSS concepts.

## Technologies Used

The following NPM packages were used to build this project:

- [Bootstrap v5.0](https://getbootstrap.com/docs/5.0/getting-started/introduction/)
- [Node-Sass](https://www.npmjs.com/package/node-sass)

## Setup

To run this project locally, clone the repository and install the necessarry dependencies using npm:

```
$ git clone git@github.com:kevin-aminzadeh/02-bootstrap-responsive-portfolio.git
$ cd 02-bootstrap-responsive-portfolio
$ npm install
```

Once NPM has finished installing the Bootstrap and Node-Sass packages, run the following command to initiate the Node-Sass daemon process:

```
$ npm run sass
```

This process will automatically detect changes made to the project's `main.scss` Sass stylesheet and recompile it, reflecting the changes in the CSS stylesheet found in the `dist` folder.

Since this project utilizes only the Bootstrap components it requires using Sass imports, additional Bootstrap classes must be imported in the `main.scss` before they can be used in the HTML pages.

Furthermore, it's necessary for the Node-Sass daemon to be run using the above command for styling changes to be reflected correctly, as the `main.scss` stylesheet must first be compiled to CSS by Node-Sass.

## Requirements

The following list of requirements were derived from the project brief and considered when building this project:

- Functional, deployed application
- Github respository with README describing the project
- Navbar must be consistent on each page
- Navbar on each page must contain links to Home/About, Contact, and Portfolio pages
- All links must work
- Must use semantic HTML
- Each page must have valid and correct HTML
- Must contain your personalized information
- Must properly utilize Bootstrap components and grid system

## Approach

To address the project's requirements, semantic HTML elements were used to correctly structure the information presented on each page of the site. A combination of Bootstrap's component, grid and utility classes were then used to apply the desired styles and responsive behaviours to the contents of each page.

In an effort to improve the site's performance slightly, unused/redundant Bootstrap CSS classes were avoided through explicitly importing only the classes required by the site from Bootstrap's Sass library into a Sass stylesheet ( `main.scss`), as oposed to including the entire Bootstrap CSS stylesheet.

This Sass stylesheet was then compiled down to CSS using Node-Sass and linked to the pages.

## License

This project is licensed under the terms of the MIT license.
