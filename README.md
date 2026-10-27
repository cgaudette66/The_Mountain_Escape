# FinalProject

##The Mountain Escape
Where the soul awakens, and nature heals.

###Project Overview
The Mountain Escape is a fictional boutique glamping retreat designed to provide guests with a peaceful outdoor experience while enjoying the comforts of luxury accommodations. The goal of this project was to create a professional single-page website that demonstrates front-end web development skills using semantic HTML, CSS, and JavaScript while meeting all project requirements.

###Project Requirements
The project required creating a complete, fixed-width (1280px) website using only original code written from scratch.
Required features included:
--Semantic HTML structure
--External CSS styling
--JavaScript functionality
--Navigation within the page
--Light/Dark mode toggle
--Contact form with validation
--JavaScript object creation from submitted form data
--Product display section
--Number guessing game
--Organized, commented code
--HTML and CSS validation
--No console errors
--JavaScript loaded using the defer attribute
###Part 2
--jQuery Widget: Use at least one UI element like tabs, accordions, or any other interactive plugin.
--AJAX / API: Load at least three pieces of theme-related content from a third-party API or a custom JSON file.
--Web Storage: Save and retrieve data (automatically or via a user form) using localStorage or sessionStorage.
--Slideshow / Carousel: Display a minimum of three images using a jQuery plugin or another JavaScript library.

###Inspiration & Goals
Inspired by modern glamping resorts, I wanted to create a clean, welcoming website that combined beautiful visuals with interactive features. My goals were to build a professional-looking site while strengthening my HTML, CSS, and JavaScript skills.

###Development Process
I planned the site's layout and content, designed a simple nature-inspired interface, then built the website using semantic HTML, CSS, and JavaScript. Interactive features include:
--Light/Dark mode
--Amenities product display
--Number guessing game
--Contact form with validation and customer object creation

###Tools & Assets
HTML5, CSS3, JavaScript
Visual Studio Code
Chrome Developer Tools
Adobe Stock images
W3C HTML & CSS Validators

###Challenges & Reflection
The biggest challenges were form validation and JavaScript event handling. I also found configuring data persistence with web storage challenging as well. This project strengthened my understanding of front-end development, DOM manipulation, and creating a polished, interactive user experience.

###Future Improvements
With more time, I would add responsive design, online booking, an image gallery, guest testimonials, and an interactive map.

## Option 1: Independent Hand-Coding Path
Use this statement if you did not use generative AI:
- I did not use generative AI tools for this project. I used only approved course
materials, instructor examples, documentation, and my own work.
Projects that follow the independent hand-coding path may earn up to 200 out of 200
points, provided the project also follows the required GitHub workflow and meets the
project requirements.
Choosing not to use AI does not remove the requirement to show meaningful commits,
meaningful comments, testing, debugging, and understanding.
A project with no AI use but weak or missing workflow evidence may receive a much lower
score.

## GIT417 and GIT418 -- Final Project

### 03AUG26
Started with my previous GIT417 project as the base for this final project. Before adding new features, I reviewed the existing HTML, CSS, and JavaScript to identify issues that needed to be corrected or improved for the new requirements.

Required features from GIT417 included:
- Semantic HTML structure
- External CSS styling
- JavaScript functionality
- Navigation within the page
- Light/Dark mode toggle
- Contact form with validation
- JavaScript object creation from submitted form data
- Product display section
- Number guessing game
- Organized, commented code
- HTML and CSS validation
- No console errors
- JavaScript loaded using the defer attribute

## GIT418 -- Final Project

### 03AUG26
Fixed the 2 issues that were identified in the GIT417 final Rubric
1. HTML - Valid/Semantic
    - comment - No skip navigation link for keyboard users
2. JS - Element Choice 2 OR Continue Cost Calculator
    - comment - The output HTML contains a malformed closing < h3 > tag, which could affect rendering. In this case it doesn't.

### 07AUG26 - 09AUG26
#### WEB STORAGE
Work on the web Storage for the last few days to get it to work properly. Created web Storage and built it off of the existing form. I referred to the module 4 activity. Added modifications that code for my specific uses.
- separated out first and last name from the full name form input
- added the error inputs and new regex for both
- created a user object for each of the form fields
- added to check local storage to see if the user wants to rewrite or keep the stored user information
- if no user is in save the user information locally and display the information
- added reset form function
- Display user information to HTML -- show contact preferences
- fixed improper syntax for console.log in light and dark mode
- added event handler for onload
- this section i worked on for many days as I was going back and forth on which method to use with the current code I had and integrating the new code

### 09AUG26
#### jQuery WIDGET/PLUGIN
Added accordion widget to js code and appropriate files to headers. To be added to HTML
-jquery-ui.css
-jquery-3.7.1.js
-jquery-ui.js

### 09AUG26
#### 1.1 - displayUser Function Update
- Removed the Thank you message from the HTML
- added messageType to the displayUser function
- messageType tells the function which message to display.
- "thankYou" is used after a new form submission.
- "welcomeBack" is used when a saved user returns.
- removed redundant style from css
- fixed displayUser welcomeBack if user clicks cancel by adding displayUser("welcomeBack") after hiding modal

#### 1.2 - API
- Purpose: Retrieves 10 random bird observations from the iNaturalist API.
- Created an asynchronous function so await can be used.
    - Sends a request to the iNaturalist observations API.
    - https://api.inaturalist.org/v1/docs/#!/Taxa/get_taxa
    - used this page to create endpoint https://www.inaturalist.org/observations/identify
    - also found useful information on the forum https://forum.inaturalist.org/
    - Converts the API response into usable JavaScript data.
- Created a simpler object for each bird containing:
    - id — observation ID
    - species — scientific name
    - commonName — common name
    - image — bird photo URL
    - url — link to the iNaturalist observation
- Runs the function and waits for the returned data.
- Displays the retrieved birds in the browser console.
- tested log this and it works

#### 1.3 - Updated Web Storage js
- reset form after form update is cancelled
- replaced displayUser(); with displayUser("thankYou"); on replace local user with new user information

#### 1.4 - API test data
- testing API data. Ready to build HTML

#### 1.5 - API and  accordion widget
- Added html to display bird data to html 
- added event handler to display data for birds when you click on nature guides
- added div accordion widget to nature guide section

#### 1.6 - API, CSS, HTML 
- pulled plants from iNaturalist
- combined bird and plant event handler
- pulled only research grade post from iNaturalist
- replace the default square image
- removed unused css #welcomeMsg styles
- added accordion styles to customize
- added Nature Guide section styles including image sizes and grid for display

#### 1.7 - API, CSS
- added random order to birds
- updated various styles in Nature Guide for better styling
- updated readme

#### 1.8 -- Swiper and minor code tweaks in HTML, CSS, js
- added jQuery js and css files to support swiper
- added gallery with 3 images
- changed photos=true to has[]=photos as that seems to be more common
- removed the h3 headers in the output, they seemed unnecessary and redundant with the accordion
- added js section SLIDESHOW/CAROUSEL WITH jQuery PLUGIN -- the developer page was straight forward
- removed showSection home on load -- seemed unnecessary
- added swiper css