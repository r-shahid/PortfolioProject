# Project Overview

## Project Schedule

This schedule keeps track of my progress throughout the week.  


|  Day | Deliverable | Status
|---|---| ---|
|MON| Project Description | Incomplete
|MON| Wireframes / Priority Matrix / Timeline | Incomplete
|TUE| Core Application Structure (HTML, CSS, etc.) | Incomplete
|WED| MVP & Bug Fixes | Incomplete
|THU| Final Touches | Incomplete
|FRI| Present | Incomplete

<!-- Change Incomplete to Approved -->

## Project Description

My portfolio website will include a short bio, links to all my projects, and a contact form. The layout I have in mind will highlight my best/favorite project while showing recent projects in a carousel. I'm inspired by blogs like [EggCanvas](https://www.eggcanvas.com/) and my friend's [personal website](https://www.isabelcalkins.com/). I find their layouts really appealing and modern, which I hope to embody in this project. I'm also taking elements from [my own website](https://rianashahid.com/about), which was created on pre-bulit templates that don't require much coding knowledge. I'm not at a place where I can recreate the entire site from scratch, but I really like the layout I have on my About page, so I plan on doing something similar for my Desktop version. 

## Google Sheet

Click [here](https://docs.google.com/spreadsheets/d/1F6TgKH1HQ4Y9KlbVs1zh_r9-1yZ6eSXrkG6DpTmO1g8/edit#gid=0) for all my projects.

## Wireframes

* [Mobile](https://i.imgur.com/RDNHl1k.png)

 A single-column layout with projects at the top and a long bio and contact form at the bottom. Menu shows as a hamburger icon and clicking each section scrolls down the page.

* [Tablet](https://i.imgur.com/DPxS9z3.png)

 Similar to the Mobile version, projects are at the top and a bio and contact form are at the bottom of the page. Full nav bar instead of a hamburger icon. 
 
* [Desktop](https://i.imgur.com/R0TOVMO.png)
 
 Unlike the other two versions, my bio is at the top. I felt this would be more appropriate for desktop because it's easier for users to scroll down to get to the projects. On a smaller screen, where users will probably spend less time per page, it's better to have projects at the top, to make sure viewers will see it. 

## Time/Priority Matrix 

[Link](https://res.cloudinary.com/jkeohan/image/upload/a_270/v1591621734/project1_matrix_ocy5gc_h1kg0m.jpg)

Include a full list of features that have been prioritized based on the `Time and Priority` Matix.  This involves drawing a a square.  In the middle of the square, on the x axis draw a line.  The most left part of the line should start with 0hrs and the end of the line should include 2hrs.  This line will be used to estimate how much time any one feature will take to complete. 

Now draw a vertical line on the y axis.  The top of this line should have `High` and the bottom `Low`.  This line will be used to assign a priority to to each feature you wish to include in the project.  

Now create a separate list starting with A and assign it one of the features.  Continue to assign each feature a letter.  Once complete add each letter to the matrix assigning based on what your feel it's prioirty is an how long it will take to implement. If any one feature takes longer than 2hrs to complete than break it down into smaller tasks and reassign them a new letter. 

Once complete tally up the time and determine how long the project will take to complete. Now break those features into MVP and PostMVP so you can guarantee you will have a fully functioning project to demo. 

### MVP/PostMVP - 5min

The functionality will then be divided into two separate lists: MPV and PostMVP.  Carefully decided what is placed into your MVP as the client will expect this functionality to be implemented upon project completion.  

#### MVP (examples)

- Pull data using google json api
- Render data on page 
- Allow user to choose favorites 
- Save their choices in firebase

#### PostMVP 

- Anything else that is not MVP

## Functional Components

Based on the initial logic defined in the previous sections try and breakdown the logic further into functional components, and by that we mean functions.  Try and capture what logic would need to be defined if the game was broken down into the following categories.

Time frames are also key in the development cycle.  You have limited time to code all phases of the game.  Your estimates can then be used to evalute game possibilities based on time needed and the actual time you have before game must be submitted. It's always best to pad the time by a few hours so that you account for the unknown so add and additional hour or two to each component to play it safe.

#### MVP
| Component | Priority | Estimated Time | Actual Time |
| --- | :---: |  :---: | :---: | 
| Hamburger | H | 1hr | hr |
| Project Previews | H | 3hr | hr |
| Regular Nav | H | 1hr | hr |  
| Adding Form | H | 1.5hr|  hr | 
| Other sections and flex| M | 3hr | hr|
| Working with API | H | 3hrs|  hr | 
| Responsive | H | 3hr | hr | hr |
| Social Media Icons | L | 1hr |  hr |
| Total | H | 15.5hrs| hrs |

#### PostMVP
| Component | Priority | Estimated Time | Actual Time |
| --- | :---: |  :---: | :---: | 
| Project Hover | L | 3hr | -hr | hr |
| Banner letters wiggle | L | 1hr | hr |
| Interactive Banner | M | 4hr | hr |
| Materialize | H | 4hr | -hr | hr |
| Bootstrap | H | 4hr | hr |
| Make own icon | L | 4hr | hr |
| Total | H | 20hrs| hrs |

## Additional Libraries
 Use this section to list all supporting libraries and thier role in the project. 

## Code Snippet

Use this section to include a brief code snippet of functionality that you are proud of an a brief description  

```
function reverse(string) {
	// here is the code to reverse a string of text
}
```

## Issues and Resolutions
 Use this section to list of all major issues encountered and their resolution.

#### SAMPLE.....
**ERROR**: app.js:34 Uncaught SyntaxError: Unexpected identifier                                
**RESOLUTION**: Missing comma after first object in sources {} object
