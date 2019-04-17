
# NOTES

*Importing file structure: use this template "../folder/filename"
*Select the item with a querySelector.  All would require for each to access the first index, so if there's just one dont use all.

*menue.js
-- line8 and 10 grab the elements/styles of the menu and button respectively.
-- line 1 is the function that toggles the styling for the menu open
--line 4 is the actual toggling. if that class is not present, it adds it. if it is, it removes it.
--line 13 adds a click event to the button. a listenter takes two arguments, the event (click) and a callback.  if we remove the (), it will only work ONCE, stuck on. not super sure why, but having it there will allow each click of menuButton to RETURN the anonymous function toggleMenu, so it can toggle on off every time the event triggers. 


          
NAI: ARTICLES:  SEE CODEPEN










# Newsfeed-Components

In this project we are going to be building a news feed reader. The goal is to have a collapsing menu, and expandable news articles. The HTML and CSS is already done for you, you simply need to connect the pieces. After the CSS is connected it is time to move on to building out our components using JavaScript. We will be adding common functionality and styling to build reusable components.

### Need to know:    NICE ADDITION!
* CSS (LESS):
  * @import
* JavaScript:
  * ES6 classes and the constructor function.
* DOM
  * Element selection
  * Basic DOM manipulation
  * Events and event listeners

## Set Up The Project With Git

**Follow these steps to set up and work on your project:**

* [x ] Create a forked copy of this project.
* [ x] Add your project manager as collaborator on Github.
* [ x] Clone your OWN version of the repository (Not Lambda's by mistake!).
* [x ] Create a new branch: git checkout -b `<firstName-lastName>`.
* [x ] Implement the project on your newly created `<firstName-lastName>` branch, committing changes regularly.
* [x ] Push commits: git push origin `<firstName-lastName>`.

**Follow these steps for completing your project.**

* [x ] Submit a Pull-Request to merge <firstName-lastName> Branch into master (student's  Repo). **Please don't merge your own pull request**
* [ next] Add your project manager as a reviewer on the pull-request
* [ ] Your project manager will count the project as complete by merging the branch back into master.

### Preprocessor Setup

  * Run `less-watch-compiler less css index.less` from the top level of the Newsfeed-Components folder. 
  * Open index.html in your browser


### Part 1: The Menu

* Import `Menu.less` from the correct path into index.less (follow the example for `Header.less` if you’re not sure how to write the correct path)
* Follow the instructions found in the Menu.js file to complete the JavaScript functionality.  NOTE: Start near the bottom of the page by looking for `const menu`.

### Part 2: The Articles Component
* Import `Article.less` from the correct path into index.less (follow the example for `Header.less` if you’re not sure how to write the correct path)
* Follow the instructions found in the Articles.js file to complete the JavaScript functionality.  NOTE: Start near the bottom of the page by looking for `let articles`.

### Part 3: Add Articles

* Now that we have our components built, add a few articles of your own to the HTML. Notice how our JavaScript code automatically selects the new articles and adds the styling and functionality we just built to them. This is the power of components. Write the code once and add as many components as you want all while maintaining the functionality we built!

### Stretch Goals:

If you complete the main goals of the page let's play around with some cool animation libraries.

A few things to check out: 
* Native CSS Animations. 
  * CSS has the ability to animate elements using a number of different properties. Check out `transform` and `transition`, and `animate`. A word of warning, these CSS properties will act differently on different browsers, so always read and see if you need a `browser prefix` in order to animate properly. 
  * https://css-tricks.com/almanac/properties/a/animation/
* jQuery
  * jQuery is an extremely popular JavaScript library, in fact most of the native DOM manipulation we know and love, came from the jQuery library. It is worth getting a little familiar with it. The jQuery library is massive, and part of it is an animation library. jQuery gives us a fantastic method called `.animate()`. There are also simpler methods such as `slideDown` `slideUp`, `slideToggle`, `show`, `hide` and more.
  * http://www.jquery.com
* GSAP
  * Greensock Animation Platform, is by far the most powerful of the three. It is intuitive and easy to use, and you will be amazed at the results.
  * https://greensock.com/gsap

Note: Just a reminder the stretch goals are just extra practice using the tools we have learned. These are not required. Only parts 1-3 are required portions of the project. If you do not get to the stretch goals, don't worry.

* Animation: There are many ways to animate elements on the screen corresponding to user interactions.  Read the documentation of the animation platform of your choice. Animate all of the components on click.
  * Animation Goal #1. Animate the menu opening: You will need to change the CSS for the menu in order to achieve this. Get the menu to slide in from the left side of the screen. And slide out when the button is clicked. Bonus: Get the menu to slide back out when the user clicks anywhere on the screen other than the menu. 
  * Animation Goal #2 Animate the article opening. This one is a bit trickier. You will need to change the CSS for this component as well. Animate the component so that it slides open and slides closed on each click. Update the text in the expand button to read `'Click to Expand'` or `'Click to Close'` depending on the state of the article. 

* Close Button

  Add a close (or 'read') button to each Article component. When clicked the article will disappear.

* Component Constructor
  
  Create a function that builds Article components. You are not expected to finish this. This goal is simply an exercise in thinking about how you would implement a function that took some data, created a new Article from it, and appended it to the HTML (without actually writing anything in the HTML file). This is a difficult concept to undertake, but even thinking about how you would implement it will give you a better understanding of how we use frameworks in upcoming sprints. 

* Implement a way to write your own articles using the Component Constructor and some input fields. 
