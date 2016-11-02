# Exam: HTML & CSS

### Getting Started
 - Fork this repository under your own account
 - Commit your progress frequently and with descriptive commit messages
 - All your answers and solutions should go in this repository

### What can I use?
 - You can use any resource online, but **please work individually**
 - Instead of copy-pasting your answers and solutions, write them in your own words.


# Tasks

## 1. Build a design (~90 minutes) [10 points]
Build the following profile cards according to the design provided.   
Follow the design as closely as possible.   
Commit an HTML and a CSS file to this repository.
![design](exercise-1.png)

### Assets
John Duck | Jane Duck | Pencil icon
--------- | --------- | -----------
![duck](duck.jpg) | ![duck](duck2.jpg) | ![pencil-icon](edit-icon.png)   

### Other data
  - Name font size: 28 pixels
  - Text size: 14 pixels
  - Font family: Arial, sans-serif

### Acceptance criteria
The task is accepted if:
  - The result follows design [2p]
  - The code follows style guide [1p]
  - The CSS & HTML are valid [1p]
  - The HTML considers semantic responsibilities [2p]
  - The code avoids code duplication [2p]
  - The CSS has meaningful and short selectors [2p]

Extra points for if:
  - the result is centered on the page [2p]


## 2. Understand code (~15 minutes) [2 points]
Read the following code snippet:   
What is the distance between the top-left corner of the document body and the yellow box?   
Give a detailed explanation below!   
Add your answer to this readme file, commit your changes to this repository.
```HTML
<!DOCTYPE html>
<html>
  <head>
    <style>
      body {
        padding: 0px;
        margin: 0px;
      }
      .foo {
        top: 20px;
        left: 20px;
        width: 100px;
        height: 100px;
        position: absolute;
        background: blue;
      }
      .bar {
        top: 20px;
        left: 20px;
        width: 30px;
        height: 30px;
        position: absolute;
        background: yellow;
      }
    </style>
  </head>
  <body>
    <div class="foo">
      <div class="bar"></div>
    </div>
  </body>
</html>
```
#### Your answer: [2p]
The distance between the top-left corner of body and top-left corner of the yellow box is 40 px. As blue and yellow 
boxes have position:absolute, they are on top of each other. Body does not have margin and paddig, blue box is 20 px
down and 20px right from the top-left corner, and yellow is additional 20px down and right (on top of blue). 
That's equal to 40px in total from top-left corner.

## 3. Explain concepts (~15 minutes) [4 points]


### Explain the difference between `display: block` and `display: inline` in CSS! What is `display: inline-block`?
#### Your answer: [2p]
Add your answer to this readme file, commit your changes to this repository.
display:block elements are for example div, p, heading etc. Box modell is valid for block elements, these fill out the
full width of the page, they are coming underneath each other.
display:inline elements are for example a, span etc. Box modell is not valid, margin and padding cannot be added. 
They are coming next to each other within a line. 
display: inline-block elements has both inline and block element properties. Box modell is valid - margin, 
padding, border etc can be added. 

### What is the difference between a `<section>` and an `<article>` element? Name one good example of using an `<article>`.
#### Your answer: [2p]
<section> is one special part of the site, used for e.g. highlighting information, can be part of the nav. 
Within section h1-h6 starting separately.
<article> is the text, displayed on all sites of a webpage, with the same format. E.g. a blog with several articles
