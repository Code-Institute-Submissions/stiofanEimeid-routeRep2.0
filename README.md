<h1 align="center">
  <a href="https://stiofaneimeid.github.io/routeRep2.0/" target="_blank"><img src="https://github.com/stiofanEimeid/routeRep2.0/blob/master/assets/images/routeRepLogofinal.png" alt="routeRep Logo"/></a>
</h1>

<div align="center"> 

[Visit the site](https://stiofaneimeid.github.io/routeRep2.0/)

</div>


# Stephen Byrne Portfolio

Stream Two Project: Interactive Frontend Development - Code Institute 

The routeRep travel application uses the Google Maps and Places APIs to allow users to select a location and find places to visit, stay and dine.
Users may then add these results to an itinerary. They may then continue to edit this itinerary to help plan their perfect trip. 

## Table of Contents
1. [**UX**](#ux)
    - [**Project Goals**](#project-goals)
    - [**User Goals**](#player-goals)
    - [**User Stories**](#user-stories)
    - [**Design Choices**](#design-choices)
    - [**Wireframes**](#wireframes)

2. [**Features**](#features)
    - [**Demo**](#demo)
    - [**Existing Features**](#existing-features)
    - [**Features Left to Implement**](#features-left-to-implement)

3. [**Technologies**](#technologies)

4. [**Testing**](#testing)

5. [**Deployment**](#deployment)
    - [**How to Run Code Locally**](#how-to-run-locally)

6. [**Credits**](#credits)
    - [**Content**](#content)
    - [**Media**](#media)
    - [**Code**](#code)
    - [**Acknowledgements**](#acknowledgements)

## UX

### Project Goals

#### User Goals

The central target audience for this page are people planning a trip with an interest in history, art and outdoor activities, travelling alone or as a group.

User goals are:
- use the planner section to select a city to visit, stay and dine at with ease;
- keep track of choices made. 


routeRep is a great way to meet these user needs because:
- it uses the Google Maps and Places API to provide comprehensive data on places to visit, stay and dine;
- users can keep track of their choices using the list functionality of the planner that acts as a simple itinerary;
- the controls are straightforward but plenty of guidance is provided to make sure no one is confused using the app.

#### User Stories

I aimed to design a site that captured the idea of escapism while developing site functionality that allowed users to research and plan various aspects of a trip with ease. 

As a visitor to routeRep I want:

1. to select a city and gather all the information I need for a successful trip. That means finding places to visit, stay and dine.
2. additionally, I want to keep track of my choices using a list.

### Design Choices

I intended to capture a sense of escapism and adventure with the design of the site while communicating the functionality of the site to the user in the clearest way possible. The following design choices were made with this in mind:

**Fonts**

- The font ```Righteous``` was chosen for its dynamic appearence and modern, agile feel to make headers stand out on the page. 
- The font ```Cabin``` was chosen because it complimented the Righteous font. The clean design was perfect for legibility while retaining the same modern and agile feel as the ```Righteous``` font.

**Icons**

- The icons used for the visit, stay and dine buttons in the planner were chosen for their simplicity to help convey the purpose of each button easier. The bed for the stay button and the knife and fork for the dine button are self-explanatory. An arch was used with the visit button to help convey the idea of history or impressive places to visit. 

**Colours**

- There are three main colours used in the design of the app - blue(```#bce7f6```) to represent clear skies and the sea; yellow(```#f6d9bc```) to represent sunsine; and purple(```#e7bcf6```) to compliment the other two colours. Violet rather than ```#e7bcf6``` was chosen for the logo because of its greater vibrancy.

**Styling**

- The user is greeted with a full-sized image of a forest, with the app’s brand name and logo taking up a small amount of space in the centre of the image. A mouse SVG provides an unobtrusive cue for the user to scroll down. As a redundancy, the user may click on the logo to cause the page to scroll down using jquery to the introductory section if users miss the SVG mouse. The minimalist design is intended to give the user a sense of calm, ideally the same feeling a holiday provides. 
- The triangles act as lens to the image and connective tissue between the first and second sections of the app. As lens, the speak to seeing things from new perspective while conveying a sense of energy and dynamicism.
- Directly below this image is an introductory section that provides some basic guidance about how to use the app. The app is designed to be as intuitive as possible and so the text here was kept to a minimum. A GIF displaying a walkthrough of the site is also provided to help commununicate effectively an understanding of how the site works.

**Backgrounds**

- The image is intended to provide a sense of escape; the forest is free of people or distractions and waiting to be explored.
- The white background for the introductory section and map section was chosen to improve legitbility and make the colours stand out more. The itinerary includes a colour gradient to be more visually appealling.

**Logo**

- The logo evolved from a cube to a hexagon for a cleaner look. The line across the logo creates two shapes that evoke arrows pointing in different directions - new places to visit with the help of the app.

### Wireframes

This [wireframe](https://github.com/stiofanEimeid/routeRep2.0/blob/master/assets/wireframes/TA-wireframe.jpeg) illustrates early conceptions of the site. This [second wireframe](https://github.com/stiofanEimeid/routeRep2.0/blob/master/assets/wireframes/routeRepfinal.jpeg) gives an impression of the final look of the site.


## Features

### Demo

<div align="center"> 

![demo gif](https://github.com/stiofanEimeid/routeRep2.0/blob/master/assets/images/routeRepDemoLarge.gif)

</div>

### Existing Features

The app uses the Google Maps and Google Places API to provide search results about accommodation, places of interest and places to eat. Each individual result may be added to a list below the map so users can keep track of the places they wish to visit, stay or dine.


### Features left to implement 

In the future, I would like users to have the ability to save their composed itineraries in the form of a PDF. At the moment, they receive an error message contained in a modal when they click the save button. 

## Technologies Used

- This project uses HTML, CSS and JavaScript programming languages.
- [JQuery](https://jquery.com)
    - The project uses **JQuery** to simplify DOM manipulation.
- [Cloud9](https://c9.io) 
    - Developer used **Cloud9** for their IDE while building the website.
- [Bootstrap](https://www.bootstrapcdn.com/)
    - The project uses **Bootstrap** to simplify the structure of the website and make the website responsive easily.
    - The project also uses Bootstrap to provide icons from [FontAwesome](https://www.bootstrapcdn.com/fontawesome/)
- [GitHub](https://github.com/)
    - This project uses **GitHub** to store and share all project code remotely. 
- [Unsplash](https://unsplash.com/)
    - The background image used at the top of the app was found on unsplash, a stock image library.
- [Google Fonts](https://fonts.google.com/)
    - The project uses **Google fonts** to style the website fonts.
- [Google Maps](https://cloud.google.com/maps-platform/)
    - The app uses the **Google Maps API** and associated code to generate a map object in the app.
- [Google Places](https://cloud.google.com/maps-platform/places/?utm_source=google&utm_medium=cpc&utm_campaign=FY18-Q2-global-demandgen-paidsearchonnetworkhouseads-cs-maps_contactsal_saf&utm_content=text-ad-none-none-DEV_c-CRE_342707335086-ADGP_Hybrid+%7C+AW+SEM+%7C+BKWS+~+Google+Maps+Places+API+EXA-KWID_43700042842848036-kwd-22859391737-userloc_1007850&utm_term=KW_google%20places%20api-ST_google+places+api&gclid=CMOd95rs1-ICFcGHGwodv48ANg)
    - The app uses the **Google Places API** to provide location information to the user when they are using the map. 
- [Favicon](https://www.favicon-generator.org/)
    - Favicons were generated from a screenshot of the routeRep logo using the **favicon-generator** site. 
- [QuickTime](https://support.apple.com/quicktime)
    - **QuickTime**'s screen capture feature was used to capture video of the app in use. 
- [Ezgif](https://ezgif.com/)
    - Video captured using Quicktime was converted to GIF format using the **Ezgif** site.
- [Compressjpeg](https://compressjpeg.com/)
    - The **Compressjpeg** site was reduced to reduce the file size of the background-image used at the top of the app.
- [Autoprefixer](https://autoprefixer.github.io/)
    - The **Autoprefixer** was used to to make sure css had all prefixes necessary to work across all browsers.
- [HTML Color Picker](https://www.w3schools.com/colors/colors_picker.asp)
    - The w3schools.com **HTML Color Picker** was used to help find colours for the app.

## Testing

Information on the testing process may be found in the [testing.md file](https://github.com/stiofanEimeid/routeRep2.0/blob/master/testing.md). 

## Deployment

The site was built using Cloud's IDE, added, commited and pushed to GitHub using the terminal. A live version of the site is hosted on GitHub pages. 

### How to Run Code Locally

In order to run a repository locally, the repository must be cloned. To clone the repository
:
1. Follow the link to the [routeRep GitHub repository](https://github.com/stiofanEimeid/routeRep2.0).
2. Under the repository name, click "Clone or download".
3. In the Clone with HTTPs section, copy the clone URL for the repository. 
4. In your preferred IDE, open the terminal.
5. Change the current working directory to the location where you want the cloned directory to be made.
6. Type ```git clone```, and then paste the URL you copied in Step 3.
```console
git clone https://github.com/USERNAME/REPOSITORY
```
7. Press Enter. Your local clone will be created.

Further reading and troubleshooting on how to clone a repository from GitHub may be found [here](https://help.github.com/en/articles/cloning-a-repository).

To cut ties with this repository, type ```git remote rm origin``` into the terminal of your editor. In order to verify the terminal has been removed, type ```git remote -v``` to determine which remotes are still connected. 

## Credits

### Content 

- All site copy was written by me. Logo was also designed by me and brand name and tag line were written by me.

### Media

- The photo is by Lukasz Szmigiel and was found on Unsplash, a stock image library. It was later compressed using [compressjpeg.com](https://compressjpeg.com/).

### Code

- The SVG mouse found at the top of the site was initially found on page one, entry no. 3 of this [css animations page](https://www.creativebloq.com/inspiration/css-animation-examples)
which displayed code from this codepen: [SVG mouse](https://codepen.io/matchboxhero/pen/gGdJYo "SVG mouse"). Minor changes were made in relation to positioning on the page.

- The planning section’s map functionality was modelled after the code contained in the [Google Maps API documentation](https://developers.google.com/maps/documentation/javascript/examples/places-autocomplete-hotelsearch), 
specifically an example about how to search for hotels by selecting a country and a city. It was modified to include searches for places of interest and places to dine. Changes were also made to allow users to push results to a list. 

- The jQuery code that causes the three div elements in the information section to fade in on scroll was found here:
[FadeIn on Scroll(jQuery)](https://jsfiddle.net/tcloninger/e5qaD/).

- The triangle divs used to create lens effects were generated using this [triangle generator site](http://apps.eky.hk/css-triangle-generator/) before changing the size, colour and opacity. 

- The GIF demonstrating how to use the planner was shot with the capture screen feature of QuickTime and converted to GIF format using this site, [ezgif.com](https://ezgif.com/).

- The site's favicon was generated using [favicon-generator.org](https://www.favicon-generator.org/).

- The text gradient code was found at [css-tricks](https://css-tricks.com/snippets/css/gradient-text/).

- Smooth scroll functionality was found at [abeautifulsite](https://www.abeautifulsite.net/smoothly-scroll-to-an-element-without-a-jquery-plugin-2).

- Map styles, [Pale Dawn](https://snazzymaps.com/style/1/pale-dawn), are by Adam Krogh.

- Finally, this README.md was written with the help of this [guide](https://github.com/AJGreaves/familyhub/blob/master/README.md#code).

### Acknowledgements

Thank you to friends and family for testing the app and for the guidance provided by my mentor. 

[**Jump to top &uarr;**](#table-of-contents)
