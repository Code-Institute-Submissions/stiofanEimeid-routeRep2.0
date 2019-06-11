# routeRep - Testing details

[Main README.md file](README.md)

## Table of Contents

1. [**Automated Testing**](#automated-testing)
    - [**Validation services**](#validation-services)
2. [**Client Stories Testing**](#client-stories-testing)
3. [**Manual Testing**](#manual-testing)
    - [**Testing undertaken on desktop**](#testing-undertaken-on-desktop)
    - [**Testing undertaken on tablet and phone devices**](#testing-undertaken-on-tablet-and-phone-devices)
4. [**Bugs discovered**](#bugs-discovered)
    - [**Solved bugs**](#solved-bugs)
    - [**Unsolved bugs**](#unsolved-bugs)
5. [**Further Testing**](#further-testing)

## Automated Testing

### Validation services
The following validation services and linter were used to check the validity of the website code.
- [W3C Markup Validation]( https://validator.w3.org/) was used to validate HTML.
- [W3C CSS validation](https://jigsaw.w3.org/css-validator/) was used to validate CSS.
- [JSHint](https://jshint.com/) was used to validate JavaScript.


## Client stories testing

The following section goes through each of the user stories from the UX section of [README.md](README.md)

**As a user I want**

1. **to select a city and gather all the information I need for a successful trip. That means finding places to visit, stay and dine.**
    
The Google Places API documentation provided an example of code that allowed users to find a hotel in a selected city. After choosing a country from a dropdown menu, the map would pan to that country. When the user entered the name of a city into the search box the map would pan to that city and markers would drop on the map, indicating hotels in the chosen city.
I modified the code so that when the user selected a country or a city, markers would not immediately appear indicating hotels. Instead, I took the code that identified hotels and added it to an event listener. This function would only be triggered when the user clicked the button the event listener targeted, labelled "stay". I repeated this process for buttons labelled "visit" and "dine", that
displayed markers on places of interest and places to eat on the map when clicked. The API identifies places to put markers based on the ```types``` property in the search object. The ```types``` ```lodging``` and ```restaurant``` were conveniently available already, but there was no equivalent for places of interest or tourist attractions. Instead, I included multiple types that fell under this umbrella, including 
```museum```, ```park```, ```zoo```, ```art_gallery```, ```church``` to provide satisfactory results.
 
The app asks users to choose a country and then enter the name of a city in that country. The map responds to each request, panning to the country and then to the city. The user then chooses from one of three options what they’d like to search for in the city, someplace to visit, someplace to stay, or someplace to dine. Markers are dropped into the map and the corresponding search results are displaced in a table alongside the map. Hovering over the markers causes a small text box to pop up providing some more information about the target. 
 
The dropdown menu offers the user the choice between twenty-four suggested countries across five continents. However, if the user wishes to choose a city located outside of those featured in the dropdown menu, they may choose the ```all``` option from the same menu. They may now search for any city in the world. 

When the user types into the city search box, suggestions correspond to cities in that location.

If the user clicks the visit, stay or dine button without first selecting a country and/or city, Montluçon, France will act as the default city.

Alternating between different options to visit, stay and dine lays down relevant markers but also erases markers from the previous choice. Nevertheless, by adding locations to the itinerary, users can keep track of their choices.

Changing city does not affect items contained in the itinerary although users may find it difficult to differentiate between choices relating to different cities. 

Markers dropped into the map correspond to the correct location and the small corresponding text-box that appears when a user clicks on a map marker is also accurate.

The autocomplete box used to search for cities in a given country relies on two-letter codes to narrow the search to the correct country, codes supplied by the ISO(International Organization for Standardization). Thus, the value of the option selected must conform to the value used by the search box. Issues arose when
I used my own codes. For example, 'IR' for Ireland in the HTML and JS. However, this code represented 'Iran' for the searchbox under ISO rules. Therefore, if a user selected Ireland they would only be given the choice to select cities from Iran. The correct country codes were identified using this [site](https://www.worldatlas.com/aatlas/ctycodes.htm). Each code was tested to ensure accuracy. 

2. **to keep track of my choices using a list.**

The corresponding search results are accompanied by a span containing a plus button that allows users to add places of interest to them to an itinerary at the bottom of the page. 

Clicking on the span containing the plus symbol in the results table will add that result to the itinerary. Clicking on the cross contained in the span symbol will remove that item while clicking the name itself will toggle a ```strike-through``` css property on the relevant name. Once the user is finished, she will have a list of all the places of interest to her. 

The user may add the same option multiple times. Duplicates, mistakes or choices no longer desired may be deleted by clicking on the close span appeneded to the end of each list item.

If the user clicks the save button, whether or not the list is populated a modal will be displayed. The modal gives the user an error message saying that the site is unable to save the list.

## Manual testing

Below is a detailed account of all the manual testing that has been done to confirm all areas of the site work as expected. 

### Testing undertaken on desktop and laptop

All steps on desktop and laptop were repeated in browsers: Chrome, Firefox, Safari, Opera and Internet Explorer and on two different desktop screen sizes.

1. Responsiveness
    - The results table sits alongside the map on larger devices as PC and laptop. 

### Testing undertaken on tablet and phone devices
All steps below were repeated to test mobile specific elements on the developer's OnePlus 6 mobile phone and tablet. 
Tests also undertaken in the Chrome Developer Tools device simulators on all options and orientations.

1. Responsiveness
    - The results table is hidden and appears directly under the map only when the user selects the visit, stay or dine buttons.

This site was tested across multiple browsers (Chrome, Firefox, Safari, Opera and Internet Explorer) in Google Dev tools(Galaxy S5, Pixel 2/Pixel 2 XL, iPhone 5/SE/6/7/8 Plus, X, iPad and iPad Pro) and on the developer's mobile (OnePlus 6, in Chrome, Safari and Opera) to ensure compatibility and responsiveness.

## Bugs discovered

### Solved bugs

When testing the site on a OnePlus 6, I noticed that the second triangle ended in the corner of the screen rather than the corner of the image. As a result, it appeared to be floating partway up the side of the image. Setting the ```bottom``` property to ```0``` did not resolve the issue.
I fixed this issue by using a ```calc``` value for this triangle's ```top``` property in css. The triangle's ```height``` was ```200px``` and the background image's ```height``` was ```100vh```, so I set ```top``` to ```calc(100vh - 200px)```, placing the triangle the correct distance from the bottom of the image. 
When a phone was turned sideways the SVG mouse would appear on top of the logo. To fix this the element's ```display``` property was set to ```none``` and a media query was created setting its ```display``` property to ```inline``` on screens with a ```min-height``` of ```640px```.

### Unsolved Bugs

Marker images from Google are blocked on browsers not in incognitio mode. ```Failed to load resource: net::ERR_BLOCKED_BY_CLIENT``` appears in the console. Appears to be a cache/cookie issue but can only get around it by switching to incognito mode.

Attempts to repurpose duplicate code into a single function at lines 273-297, 308-332, 343-367 of main.js ran into difficulties when pushed to GitHub and displayed on GitHub pages. The markers fail to display and ```Uncaught TypeError: b is not a function``` appears console when the page.

## Further Testing

Family and friends were asked to try the app on their devices. This insight was invaluable for improving site usability. 

[**Jump to top &uarr;**](#table-of-contents)
