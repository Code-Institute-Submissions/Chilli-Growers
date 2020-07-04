**Milestone Project 1: User-Centric Frontend Development - Code Institute**

# Chilli Growers.

A website designed to provide information to users on how to grow chilli plants. Will also include a section on recommended chilli types with links to the related wikipedia pages.
The userbase will mostly be beginner growers looking to start their own plant.

# UX

To make a responsive website for beginner chilli growers, that provides a guide and suggestions for what to grow.

The initial idea was hand drawn:

[Hand Drawn Wireframe](https://github.com/bob134552/Chilli-Growers/tree/master/wireframe/Initial-Hand-Drawn-Wireframe.pdf)

Balsamiq was used the create the following wireframe:

[Balsamiq Mobile and Desktop Wireframe](https://github.com/bob134552/Chilli-Growers/tree/master/wireframe/Chilli-Growing-Website.pdf)

## The Strategy Plane

The objective is to create a site with the goal to guide and assist a user looking to begin growing chilli plants.
The immediate needs would be a guide and provide a variety of options available for the user.

## The Scope Plane

The site's requirement will be to inform and educate the user in a simple manner such that it doesn't feel like they are being overloaded with information.
To acheive this a guide using tabs to display different information is used along with a gallery to display choices for the user.

In short what is required:

- A Guide
- A Gallery
- A Callout

## The Structure Plane

The general layout would be a single scrolling page with a navigation section to move to different points throughout the site.
In order to display each section in a fluid way the site would be organized from callout to gallery (Callout to Why Grow to Guide to Gallery).

## The Skeleton Plane

The skeleton of the site was designed using Balsamiq and can be found in the link above.

## The Surface Plane

The project is a single scrolling page which has a full veiw height image with a callout and button that opens a modal for the user to subscribe with.
The navigation bar is set to the top of the page and is always available for the user to be able to move around the page with ease.

The site is split up into 3 main sections which are in an order from what the user should see first into finally showing them a gallery of which they can make a choice from.

After a look at different guide and garden store sites the font "PT Sans" was chosen as it looked like a good fit for a guide site and
"Balsamiq Sans" for titles complimented the body font.

Each banners color before each section was chosen to represent the [Scoville Scale](https://en.wikipedia.org/wiki/Scoville_scale) beginning from green to red.

## User Stories

- As a user, I want to be able to move around the site easily on mobile and desktop.
- As a user, I want to have easy access to a guide that is simple to interact with.
- As a user, I want to be able to sign up for future updates.
- As a user, I want to see a variety of chillies I can choose and see infromation on.

# Features

The website has 4 main sections:

- A home section containing a navbar to help navigate the site and a callout with button to allow the user to sign up for updates.
- A reasons sections detailing why the user should grow their own chillies.
- A guide section that uses vertical pills and tab panes to present information in a easy way that saves space.
- A gallery section that contains 6 (4 on mobile) different varieties of chillies that the user can get information on.

## Existing Features

- Feature 1 - Collapsible Navigation Bar, this allows the user to navigate the site with ease.
- Feature 2 - Guide using tab pane, This allows the user to have access to a growing guide that doesn't require scrolling to see relevant information.
- Feature 3 - Modal with button, This allows the user to submit their email and name to let the user sign up for future updates and news.

## Features Left to Implement

- Add a shopping cart to sell the recommended chillies.
- Add a feature that remembers which tab they were on before leaving the page so they can continue from where they left off on the guide.
- Add in a sign in instead of subscribe for people to be able to log in and buy seeds.

## Technologies Used

- [Balsamiq](https://balsamiq.com/)
  - For a basic wireframe mockup.
- [HTML](https://en.wikipedia.org/wiki/HTML)
  - To create the site.
- [CSS](https://en.wikipedia.org/wiki/Cascading_Style_Sheets)
  - To create custom styles.
- [JQuery](https://jquery.com)
  - To simplify DOM manipulation.
- [Bootstrap](https://getbootstrap.com/)
  - For better responsiveness.
- [Font Awesome](https://fontawesome.com/)
  - To add icons to navbar and reasons section.

# Testing

The site was tested on several devices to ensure responsiveness throughout. 

Devices included: Samsung Galaxy S10+, iPhone X, Samsung Galaxy Tab A, Desktop PC (custom built) and MacBook Air.

## Testing based on user stories:

## As a user, I want to be able to move around the site easily on mobile and desktop.

1. Clicking on each part of the navigation bar allows the user to move to different parts of the site.

   1. Click on chilli growers on navbar, nothing happens when at the top of the site but returns to top if on other parts of site.
   2. Click on Why Grow? scrolls the site down to the reasons section.
   3. Click on Growing Guide scrolls the site to the guide section.

2. In mobile view the navigation bar will collapse into a toggle button that can be used to move around the site also.
   1. Clicking on the toggler expands the navbar.
   2. Clicking on each link brings the respective section into view.

## As a user, I want to have easy access to a guide that is simple to interact with.

1. Guide section.
   1. Clicking on each tab changes the information that is displayed.
   2. Clicking on each tab shows which tab pane is open, indicated by a black border around the tab.

## As a user, I want to be able to sign up for future updates.

1. Subscribe button and modal.
   1. Try to click on subscribe button opens a modal asking for users first name and email.
   2. Try to submit with empty fields and getting error messages about required fields appear.
   3. Try to submit with either Full name or email empty and getting error message when either isn't filled in.
   4. Submit form with both Full name and email correctly input and modal closes and returns to page.
   5. Trying to click on the close button or outside of the modal closes modal and returns to the main site.

## As a user, I want to see a variety of chillies I can choose and see information on.

1. Gallery
   1. Try to click on a chilli (image or name) opens a seperate browsers tab that is linked to the respective chillies wikipedia page.


# Bugs and Problems

## Scrolling to wrong point in correct section.

Initially clicking on each navbar link would bring you to the correct section but with the navbar covering part of the heading for the section.
This was fixed by adding in a banner of equal height to the navbar before each section and having the links on the navbar navigate to each banner.

## Images not fitting within their respective containers.

Images in the gallery section would not fill the container they were in, this was resolived by using the CSS: object-fit: contain.

## Fonts not scaling down on smaller screens.

A lot of text was not scaling down and as such would overflow over other elements or disappear,
this was fixed by using the "[calc](https://www.w3schools.com/cssref/func_calc.asp)" function in order to help with scaling.

## Navbar transparency

During the styling of the navbar, I unable to find a way to make the background transparent as when the opacity of the background was set it would turn white.

## Validaton and Beautify

The code for index.html and style.css was beautified using [Code Beautify](https://codebeautify.org/).

In addition, the [W3C CSS Validator](https://jigsaw.w3.org/css-validator/) and [W3C HTML Validator](https://validator.w3.org/#validate_by_input+with_options) was used to validate the code.

## How the project works

The project is designed to be a single scrolling page, with the use or a navbar that it stuck to the top to allow ease when moving around.
On larger screen there is padding to all sections so content looks more centralized.

On smaller screen sizes the navbar collapes into a toggle button which can be used to show and hide each navbar link for easier movement around the page.
In addition, the reasons section changes from 4 elements in a single row to 2 elements per row on smaller screens.
Similarly on smaller screens 2 of the chillies are hidden and the layout becomes a single element per row to avoid filling the page too much and images from
scaling down too much.

# Deployment

The project was deployed through Github pages, from the master branch, and can be found [here](https://bob134552.github.io/Chilli-Growers/). 

Additionally the site will be updated after any git push to the master branch.


### How to run code locally.

To run the site locally you can visit [here](https://github.com/bob134552/Chilli-Growers) and clone the code by copying HTTPS code provided into a code editor of your choice.

# Credits

## Content

Majority of content was written by me.

Chilli descriptions adapted from [Pepper Scale](https://www.pepperscale.com/)

## Media

- Images within the guide were taken by me.
- Some photos were obtained from google images filtering by free license.

## Acknowledgements

- My wife for suggestions on what content to add and help in color co-ordination.
- My mentor for suggesting making a single page site instead of multiple pages.