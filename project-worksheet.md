# Project Overview

## Project Schedule

This schedule keeps track of my progress throughout the week.  


|  Day | Deliverable | Status
|---|---| ---|
|MON| Project Description | Complete
|MON| Wireframes / Priority Matrix / Timeline | Complete
|TUE| Core Application Structure (HTML, CSS, etc.) | Complete
|THU| MVP & Bug Fixes | Complete
|THU| Final Touches | Complete
|FRI| Present | Incomplete



## Project Description

My portfolio website will include a short bio, links to all my projects, and a contact form. The layout I have in mind will highlight my best/favorite project while showing recent projects in a carousel. I'm inspired by blogs like [EggCanvas](https://www.eggcanvas.com/) and my friend's [personal website](https://www.isabelcalkins.com/). I find their layouts really appealing and modern, which I hope to embody in this project. I'm also taking elements from [my own website](https://rianashahid.com/about), which was created on pre-built templates that don't require much coding knowledge. I'm not at a place where I can recreate the entire site from scratch, but I really like the layout I have on my About page, so I plan on doing something similar for my Desktop version. 

## Google Sheet

Click [here](https://docs.google.com/spreadsheets/d/1F6TgKH1HQ4Y9KlbVs1zh_r9-1yZ6eSXrkG6DpTmO1g8/edit#gid=0) for all my projects.

## Wireframes

* [Mobile](https://i.imgur.com/CBIkFcr.png)

  A single-column layout with projects at the top and a long bio and contact form at the bottom. Menu shows as a hamburger icon and clicking each section scrolls down the page.

* [Tablet](https://i.imgur.com/DPxS9z3.png)

  Similar to the Mobile version, projects are at the top and a bio and contact form are at the bottom of the page. Projects displayed in two columns and full nav bar instead of a hamburger icon. 
 
* [Desktop](https://i.imgur.com/R0TOVMO.png)
 
  Unlike the other two versions, my bio is at the top. I felt this would be more appropriate for desktop because it's easier for users to scroll down to get to the projects. On a smaller screen, where users will probably spend less time per page, I wanted to keep projects at the top, to make sure viewers will see it. 

**UPDATE**  
After seeing how the page looked, I ended up getting rid of the full-width project I had underneath the carousels. I also opted to leave my About section at the bottom of the page for all versions and implemented a parallax scrolling element at the top of my desktop version. 

## Time/Priority Matrix 

[Link](https://i.imgur.com/1SMaUfc.jpg)

### MVP/PostMVP

#### MVP (examples)

* Core Structure
* Flexbox
* Navigation Bar/ Hamburger
* Responsive Design
* Working with API
* About Me
* Contact Form
* Styling/Images
* Icons

#### PostMVP 

* Carousel
* Show Project Description on Hover
* Make Logos
* Incorporate Bootstrap
* Parallax Scrolling

## Functional Components

#### MVP
| Component | Priority | Estimated Time | Actual Time |
| --- | :---: |  :---: | :---: | 
| Core Structure | H | 3hr | 4hr |
| Flexbox | H | 2hr | 1.5hr |
| Nav Bar/Hamburger | H | 1hr | 2hr |  
| Responsive Design | H | 3hr|  4hr | 
| Working with API| M | 3hr | 4hr|
| Contact Form | M | 2hrs|  1.5hr | 
| Social Media Icons | L | 1hr | 1hr |
| About Me | M | 1hr | 1hr |
| Styling/Images | M | 3 hr | 3hr |
| Total | - | 19hrs| 21hrs |

#### PostMVP
| Component | Priority | Estimated Time | Actual Time |
| --- | :---: |  :---: | :---: | 
| Carousel | H | 3hr| 2hr | 
| Show Project Desc on Hover | M | 3hr | 4hr |
| ~~Materialize~~ | ~~H~~ | ~~4hr~~ | ~~hr~~ |
| Bootstrap | H | 4hr | 4hr |
| Make Logo Images | L | 2hr | 1hr |
| Total | - | 16hrs| 11hrs |

## Additional Libraries
This section will contain all supporting libraries.
* Carousel made with [Bootstrap](https://getbootstrap.com/docs/4.0/components/carousel/)
* Contact form submissions facilitated by [Formspree](https://formspree.io/forms)
* Logos and non-project images from [Canva](https://canva.com)
* Icons from [FontAwesome](https://fontawesome.com/icons?d=gallery&m=free)

## Code Snippets

An easier way to manage colors throughout my CSS files:
```
:root {
  --blue: #19647E;
  --eggplant: #674857;
  --timberwolf: rgb(209, 205, 197);
  --carmine: #B3533E;
  --rich-black: #111A29;
}
```
I called each color by var(--name) instead of copy/pasting the hex code every time. (from the Intro to jQuery lesson)
***
Here's how I got the parallax scrolling effect:
```
.hero-image {
        display: block;
        background-image: url("images/cover_image\ \(1\).png");
        min-height: 900px;
	    width: 100%;
	    background-attachment: fixed;
	    background-position: center;
	    background-repeat: no-repeat;
	    background-size: cover;
    }
```
***
An attempt at making each project image clickable (see issue from 9/16): 
```
$('.embedprojects').click(function() {
			window.location.href = ent.gsx$link.$t
		 });
```
While this wasn't successful, I liked that it _sort of_ did what I wanted, even though it wasn't quite what I expected. Ultimately, I didn't have enough time to keep playing with this approach and had to make the projects clickable another way, but I would like to return to this in the future and try to figure out how to make it work. 

Here's how I actually got the project links to work. The images themselves are not clickable, but now there's at least a working link:
```
.project-img {
    opacity: 1;
    display: block;
    width: 100%;
    height: auto;
    backface-visibility: hidden;
}

.embedprojects:hover .project-img {
    backface-visibility: visible;
}
```

## Issues and Resolutions

**9/14**  
* Bootstrap's breakpoint for mobile (576px) was smaller than the breakpoint I had set (768px)

  My original navbar (bootstrap) was expanding from a hamburger to a regular navbar much sooner than the rest of the page. I initially just changed my mobile breakpoint to 576px, but I ended up not using Bootstrap's navbar at all, so I changed my breakpoint back to the original value.

**9/15**  
* My footer overlapped the end of the content above it only when in a wider screen. I implemented some weird grid setting and it seems to have fixed it.

  body contains main and footer. I assigned main to the first row and footer to the second:  
   ``` 
   body {
        display: grid;
        grid-template: 23fr 1fr / 100%; 
    } 
    ```
**9/16**
* Implemented code to show project descriptions on hover, but this made the View Project links unclickable. As an alternative, I tried to make each image a link, but this linked every project to that of the last project added.

  The problem with my first attempt was that hovering over the image changed the opacity, revealing the project title, description, and link, but they were still "hidden" behind the image, so I could not actually click on them. I made it so hovering over the image toggled backface-visibility from hidden to visible so that I could now click on the View Project link.

**9/17**  
* I kept having more issues with overlapping divs, so I got rid of the grid layout on the entire page and only used it where necessary. At this point, it was hard to keep track of exactly where I used grid vs flexbox, so I rewrote the html and css from scratch, cutting down redundant code. This fixed all the problems I was having with the layout, so I must have had some style rules that were messing everything up.
* My CSS file was getting unmanageably long, so I separated it by screen size
<!-- #### SAMPLE.....
**ERROR**: app.js:34 Uncaught SyntaxError: Unexpected identifier                                
**RESOLUTION**: Missing comma after first object in sources {} object -->
