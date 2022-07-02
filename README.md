# Michael's First Attempt Portfolio


## Table of Contents

- [Description](#description)
- [Technologies](#technologies)
- [Deployed Link](#link)
- [Usage](#usage)
- [User Information](#userinformation)
- [Credits](#credits)
- [License](#license)

## Description
A one stop shop for all things Michael Wence. When landing on the page you are greeted by a lovely photo and mini bio of myself. Using css grid I created a framework that I can build upon to display more about myself. There are areas for links to my professional pages, like gitlab and linkdin, as well as ones to my deployed projects. All featured in a simple but stylish layout. 

## Technologies Used

- HTML
- CSS

## Deployed Link

[Michael Wence's Portfolio](https://mtwence.github.io/portfolio-take-1/)

## Usage

### Website Demo

![portfolio landing page](/Assets/images/portfolio.png)

### Code Snippets

The main layout of my portfolio website is styled using css grid. This grid class was applied to the '<body>` element, which acted as a container for the rest of my elements. 
#### Grid Styling:
```ruby
.grid {
    display: grid;
    height: 100vh;
    grid-template-columns: 2fr 1.5fr 1.5fr;
    grid-template-rows:.3fr 1.5fr 1.5fr .5fr;
    grid-template-areas:
    "nav nav nav"
    "bio main main"
    "bio resume links"
    "footer footer footer";
    grid-gap: 20px;
    
}
```
Using the `grid-template-areas` defined in the css styling above, I then assigned those grid areas to ids of html elements, based on where I wanted them layed out on the grid. For instance, my picture and bio are layed out in column 1:rows 2-3. Take a look at how it was done in the code snippet below. Pay attention to `grid-area: bio`.
```ruby
#bio {
    background-color: darksalmon;
    grid-area: bio; 
    display: grid;
    grid-template-columns: 2fr;
    grid-template-rows: .5fr 1fr .75fr;
    grid-template-areas: 
    "heading2"
    "avi"
    "p1" ;
  justify-items: center;
  align-items: center;
}
```
## User Information

### **Michael Wence**
[LinkedIn](https://www.linkedin.com/in/michael-wence/) |
[GitHub](https://github.com/mtwence)

## Credits

UCB - Coding Bootcamp


## License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

© 2022 Michael Wence. All Rights Reserved.