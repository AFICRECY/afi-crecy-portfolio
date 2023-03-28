# afi-crecy-portfolio 

# Online Presence Management Website

## Technology Used:
| Technology Used         | Resource URL           | 
| ------------- |:-------------:| 
| HTML    | [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) | 
| CSS     | [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)      |   
| Git | [https://git-scm.com/](https://git-scm.com/)     | 

## Description: 

[Visit Deployed Site]: XXX

It is important, as a Programmer or Software Developer, to have a portfolio which highlights your experience and past projects, skills, and or any other information that potential employers would like to see. A comprehensive portfolio with a list of your projects, previous employment and education, and a section introducing yourself will help display what you can do for future employers. Highlighting your strongest work as well as a small explanation is also paramount.


## Table of Contents: 
* Installation (Refactoring & Accessibility)
* Usage
* Credits 
* License


### Installation: 
 This project is my first programming portfolio, and while I did not have deployed projects that I could account on, I was able to create a portfolio which lists all of the technical (Software/Software Development) experience that I have already and am currently gaining. There is an initial picture, my name, title I am aiming to acquire, as well as my highest education level all sectioned within a "header" element. This "header" element was styled using flexbox properties of “display= flex” and “flex-direction=row. The content is affected also by the “justify-content: space around”. The respective code is below:

```
.header {
   display: flex;
   flex-direction: row;
   justify-content: space-around;
   font-size: 70px;
   line-height: 80%;
}
```
(in style css line 32-38)

Additionally I input a "nav" element which contains the links to the respective areas on the page. I was able to do this with a HTML "nav" id Attribute by assigning a list of anchor tags with an href value of #(Respective Section). I paired each of these nav id attributes with a id in the element on the section of the page I would like for the UI screen to scroll to when the nav link is clicked. The corresponding code is below: 

```
 <nav class="header-nav">
       <a href="#About me">About Me</a>
       <a href="#Previous Projects">Previous Projects</a>
       <a href="#Contact Me">Contact Me</a>
       <a href="#Resume">Resume</a>
   </nav>
(in index.html lines 29-34) 
```


`<h2>id="About Me" class="header"> About Me:</h2>`
(example of one of the corresponding id in the section, line 40)


Separately, within my index.html, contained within the "main" element, I was able to create an "aside" containing my “About Me”, “Contact” as well as an image of my updated Programming “Resume.” This "aside" element was given various "divs" to section off the above listed areas. Each area was styled in style.css using a class of “.header” which was styled with both the “Box-Model” as well as “Flexbox.” The styling class is detailed below: 

```
.header {
   display: flex;
   flex-direction: row;
   justify-content: space-around;
   font-size: 70px;
   line-height: 80%;
}
```

Furthermore, on the alternate side of the page I have my “Previous Projects” listed in a column order. They are collectively wrapped in a “div” element which is styled its own way, and then they are individually divided using “section” elements which hold each project. The “section” element are styled using a class of “.project”. There are also links attached to the circular images of the logo of the companies I have worked for. These links either take you to the website I used to manage or the company whose Software I have used. (These sections will be filled with actual deployed project gifs that I plan on updating in the future.) Below is a code snippet of the image link in the index.html: 

```
<a href="https://oaklandpromise.org/" target="_blank"><img class="imgcenter" src="./assets/images/ebcf-logo.png" alt="east bay college fund old-logo"></a>
```

I was also able to style the all the images on the page to, when hovered over, highlight as white/yellow. I was able to accomplish this styling with a “Pseudo Class” of “:hover”. The respective code is below. 

```
img:hover {
   box-shadow: 10px 5px 5px rgb(246, 241, 147);
}
```


I was able to utilize CSS Variables by using the "Var() Function" and was able to resue the "var(--dark)" to color all the text and any black colors with the same styling at the top of the CSS page. The example is below 

```
:root {
    --dark: #040000;
}
```
```
header {
    background: #e0bb00;
    padding: 40px;
    text-align: center;
    color: var(--dark);
}
```



Lastly I was able to adjust the screen size to the viewport screen size by adding a “Media Query” at the bottom of the CSS page. 

```
@media screen and (max-width: 768px) {


   main,
   nav {
       flex-direction: column;
   }
}
```



### Usage: 
With this portfolio potential employers can visit my deployed link and visualize some of my technical programming experience. Showcased are my education, my precious projects, information about myself and what kinds of positions I am looking for, as well as snippets of previous projects that I have worked on, companies I have worked for, as well as the types of Software that I have experience with. The intention of this portfolio is to hopefully expose myself to potential employers or project collaborators. 


## Credits:
The below links helped as a reference to styling and creating ym portfolio. 

* HTML nav id Attributes: https://www.dofactory.com/html/nav/id#:~:text=The%20id%20attribute%20assigns%20an,selector%20in%20a%20style%20sheet. 
* CSS Padding: https://www.w3schools.com/css/css_padding.asp 
* CSS Font-weight: https://www.w3schools.com/cssref/pr_font_weight.php 
* CSS Flexbox Properties: https://css-tricks.com/snippets/css/a-guide-to-flexbox/#aa-flex-wrap 
* Nav Bar Styling: https://codetheweb.blog/style-a-navigation-bar-css/ 
* Box-Sizing: https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing 
* Pseudo-classes: https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes 
* CSS Element Selectors: https://www.w3schools.com/cssref/css_selectors.php 

### License:
MIT License

Copyright (c) [2023] [Afi Nkhume-Crecy]

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



