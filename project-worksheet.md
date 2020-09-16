# Project Overview

## Project Schedule

This schedule keeps track of my progress throughout the week.  


|  Day | Deliverable | Status
|---|---| ---|
|MON| Project Description | Complete
|MON| Wireframes / Priority Matrix / Timeline | Complete
|TUE| Core Application Structure (HTML, CSS, etc.) | Complete
|WED| MVP & Bug Fixes | Incomplete
|THU| Final Touches | Incomplete
|FRI| Present | Incomplete



## Project Description

My portfolio website will include a short bio, links to all my projects, and a contact form. The layout I have in mind will highlight my best/favorite project while showing recent projects in a carousel. I'm inspired by blogs like [EggCanvas](https://www.eggcanvas.com/) and my friend's [personal website](https://www.isabelcalkins.com/). I find their layouts really appealing and modern, which I hope to embody in this project. I'm also taking elements from [my own website](https://rianashahid.com/about), which was created on pre-bulit templates that don't require much coding knowledge. I'm not at a place where I can recreate the entire site from scratch, but I really like the layout I have on my About page, so I plan on doing something similar for my Desktop version. 

## Google Sheet

Click [here](https://docs.google.com/spreadsheets/d/1F6TgKH1HQ4Y9KlbVs1zh_r9-1yZ6eSXrkG6DpTmO1g8/edit#gid=0) for all my projects.

## Wireframes

* [Mobile](https://i.imgur.com/CBIkFcr.png)

  A single-column layout with projects at the top and a long bio and contact form at the bottom. Menu shows as a hamburger icon and clicking each section scrolls down the page.

* [Tablet](https://i.imgur.com/DPxS9z3.png)

  Similar to the Mobile version, projects are at the top and a bio and contact form are at the bottom of the page. Projects displayed in two columns and full nav bar instead of a hamburger icon. 
 
* [Desktop](https://i.imgur.com/R0TOVMO.png)
 
  Unlike the other two versions, my bio is at the top. I felt this would be more appropriate for desktop because it's easier for users to scroll down to get to the projects. On a smaller screen, where users will probably spend less time per page, it's better to have projects at the top, to make sure viewers will see it. 

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
| Core Structure | H | 3hr | 3hr |
| Flexbox | H | 2hr | 1.5hr |
| Nav Bar/Hamburger | H | 1hr | 2hr |  
| Responsive Design | H | 3hr|  4hr | 
| Working with API| M | 3hr | 4hr|
| Contact Form | M | 2hrs|  hr | 
| Social Media Icons | L | 1hr | hr |
| About Me | M | 1hr | hr |
| Styling/Images | M | 3 hr | hr |
| Total | - | 19hrs| 14.5hrs |

#### PostMVP
| Component | Priority | Estimated Time | Actual Time |
| --- | :---: |  :---: | :---: | 
| Carousel | H | 3hr| hr | 
| Show Project Desc on Hover | M | 3hr | hr |
| Materialize | H | 4hr | hr |
| Bootstrap | H | 4hr | hr |
| Make Logo Image | L | 2hr | hr |
| Total | H | 16hrs| hrs |

## Additional Libraries
This section will contain all supporting libraries.

<!-- add bootstrap once I do the carousel -->

## Code Snippet

This section will contain interesting code snippets (likely will include parallax scrolling)
<!-- add code for how I embedded the content from my google sheet -->

## Issues and Resolutions

**9/14**  
* Bootstrap's breakpoint for mobile (576px) was smaller than the breakpoint I had set (768px)

  My original navbar (bootstrap) was expanding from a hamburger to a regular navbar much sooner than the rest of the page. I initially just changed my mobile breakpoint to 576px, but I ended up not using Bootstrap's navbar.

**9/15**  
* My footer overlapped the end of the content above it only when in a wider screen. I implemented some weird grid setting and it seems to have fixed it.

  body contains main and footer. I assigned main to the first row and footer to the second:  
   ``` 
   body {
        display: grid;
        grid-template: 19fr 1fr / 100%; 
    } 
    ```

<!-- #### SAMPLE.....
**ERROR**: app.js:34 Uncaught SyntaxError: Unexpected identifier                                
**RESOLUTION**: Missing comma after first object in sources {} object -->
