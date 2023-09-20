# Refacoring an index.html file to follow the accessibility standards

## About this project
This project was done as the first assignment of a codind bootcamp as part of the process to learn about HTML / CSS. I was given a functionaning HTML file and CSS file and tasked to refactor the page to meet the accessbility standards. 

As the following criteria are given to the project:
- Using Semantic HTML elements
- The heading attributes fall in sequential order
- The elements follow a logical structure independent of styling and positioning
- The icon and image elements have alt attributes
- The title element contains a concise, descriptive title

## Installation

Visit https://mitsukaichi.github.io/horiseon-refactoring/
[Screenshot](./assets/images/screenshot.png)

## How I addressed this challenge

I researched about what the semantic HTML elements are and referred to the following websites;
- [W3 School: HTML semantic elements](https://www.w3schools.com/html/html5_semantic_elements.asp)
- [Semrush Blog: Semantic HTML: What It Is and How to Use It Correctly](https://www.semrush.com/blog/semantic-html5-guide/)
- [Smashing magazine: Semantic CSS With Intelligent Selectors](https://www.smashingmagazine.com/2013/08/semantic-css-with-intelligent-selectors/)

I found the original HTML files are mainly using \<div> elements, so I updated those elements to the following elements to make it semantic HTML.
- \<header>
- \<nav>
- \<section>
- \<article>
- \<aside>
- \<footer>

By grouping each \<div> elements in to semantic elements, I could also upate the heading attributes fall in sequential order within each element. I also updated the CSS to match the updated element names.

After moving the \<ul> element in the \<header> element inside of \<nav> element, display: inline-block started to conclict with float: right in CSS and the list items aligned to the right didn't render as it should be. I did some researches and used [the flexbox property](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) to control how the elements in the header are styled to solve this issue.

As a next step, I added the alt text to the icons and images in the file using alt="". There is one background image file referred in the CSS file instead of the index.html, and I used the aria-label element to add the alt text to the background image based on [the blog article about how to add the alt text for background images](http://www.davidmacd.com/blog/alternate-text-for-css-background-images.html).

Finally, I added a title representing the content in the page in the \<title> element.


## License

MIT License

Copyright (c) [2023] [Minami Mukai]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---

© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.
