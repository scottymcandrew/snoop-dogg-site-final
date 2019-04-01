# Snoop Dogg Information and Booking Site

## This site has been created as part of my CodeInstitute milestone project for the user-centric frontend module.

### Please note the language is intentional and meant as humour - a parody of Snoop Dogg's own language style.

This site promotes the worldwide rap superstar Snoop Dogg. It contains information and samples of music and other media.

A booking form is included to make it easy to request Snoop Dogg's time for your own venue!

## UX

The original inception of the UX design came from an appreciation of two things: fluidity and simplicity. I particularly like single page websites that scroll between the sections as individual pages themselves.

I did not create a specific wireframe as the idea was a single scrolling page. The only cosideration after this was how to implement navigation functionality.

I decided to look through www.behance.net for some inspiration, which drew me to this website: http://www.hogni.com. The side bar that collapses to a simple nav bar was exactly what I had in mind, so decided to implement a similar idea.

In regards to achieving single page scrolling, after some internet searching, I found FullPage, which I decided to use the library for in my site (details on this to follow in the technologies section).

One feature I particularly like in web sites I visit, are static backgrounds. I wanted to factor this into my design, and so decided to have a profile picture of Snoop Dogg overlayed by a transparent 'tile'.

### User Stories

- As a fan, I want quick easy access to the artist's information and available media (most notably music catalogue).
- As a venue operator, I need the ability to gauge an artist's feasibility and view their work history/catalogue.
- As a venue operator, I need the ability to book the artist and provide information on the venue via a booking form.

## Features
 
### Existing Features

- Feature 1 (Landing Page) - allows users to see a bio of Snoop Dogg
- Feature 2 (News Page) - allows users to read the latest news of Snoop Dogg
- Feature 3 (Audio Page) - allows users to listen to audio of Snoop Dogg
- Feature 4 (Video Page) - allows users to view videos and bio pictures of Snoop Dogg
- Feature 5 (Booking Page) - allows users to book Snoop Dogg by filling in the booking form
- Feature 6 (Nav Bar Social Links) - allows users to reach Snoop Dogg's social media presence

## Technologies Used

The following is a list of all the technologies used in this website.

- [JQuery](https://jquery.com)
  - The project uses **JQuery** to simplify DOM manipulation. Specifically I have used this to auto-hide the top nav bar (visible on small screens) when a link is clicked. I took guidance from W3Schools: www.w3schools.com/jquery/jquery_selectors.asp

- [Bootstrap 4.3](https://getbootstrap.com/docs/4.3/getting-started/introduction/)
  - This project uses **Bootstrap** to provide the website's structure. I have relied heavily on its Flexbox utilities in particular and embed tools

- [FontAwesome](https://fontawesome.com/start)
  - This project uses **FontAwesome** for the nav bar icons

- [Google Fonts](https://fonts.google.com/)
  - This project uses **Google Fonts** for the site's fonts. Specifically Rubik and Karla

- [Hover CSS](http://ianlunn.github.io/Hover/)
  - This project uses Ian Lunn's **Hover CSS** library to provide wobble effects on the FontAwesome icons

- [FullPage](https://alvarotrigo.com/fullPage/)
  - This project uses **FullPage** to implement single page scrolling. The license is free for open source projects. Github repo: github.com/alvarotrigo/fullPage.js

- [Spotify](https://www.spotify.com/uk/)
  - This project embeds audio from **Spotify**

- [YouTube](https://www.youtube.com/)
  - This project embeds videos from **YouTube**

## Testing

1. Main Structure:
    1. Pages move either by scrolling or dragging (on phones/tablets etc).
    2. Pages can be jumped to directly by clicking the nav bar links.
    3. Pages transition smoothly.
    4. Pages with multiple pieces of content - ability to side-swipe in the form of a slide show.
    5. Social links open in a new browser tab.
    6. Small screen sizes: the side bar disappears and a top nav bar appears.

2. Main Page:
    1. Load the website. Landing page will be the home page.
    2. This page contains a bio taken from Wikipedia: en.wikipedia.org/wiki/Snoop_Dogg

3. News Page:
    1. From page load, either scroll down, click the nav link or click the navigation dots.
    2. News articles are displayed.
    3. Side-swipe for more articles.

4. Pictures Page:
    1. From page load, either scroll down, click the nav link or click the navigation dots.
    2. Bio picture is displayed.
    3. Side-swipe for more bio pics.

5. Music Page:
    1. From page load, either scroll down, click the nav link or click the navigation dots.
    2. Spotify album is dispayed.
    3. Multiple albums are available by side-swiping.

6. Video Page:
    1. From page load, either scroll down, click the nav link or click the navigation dots.
    2. YouTube video is displayed.
    3. More videos are available by side-swiping.

7. Booking Form:
    1. From page load, either scroll down, click the nav link or click the navigation dots.
    2. Booking form is displayed.
    3. Enter information and submit form successfully (this project no further action is taken, but assume this would update a backend database).

- Responsive Design:
    1. The above tests were carried out with varying screen sizes (using Chrome Dev Tools).
    2. On small screens the side-bar is hidden and a simple top nav bar is displayed.
    3. On very small screens the top nav bar background is hidden (more information on this below).

- Interesting bugs / challenges encountered:
    1. The slide (horizontal) scrolling dots were disappearing under embeds on large screens. To fix this I changed the display property to static.
    2. The top nav bar I implemented as fixed otherwise the flex containers were not centered correctly.
    3. The top nav was was covering some text on very small screens. I used a media query to remove the coloured background in these situations.
    4. Certain pages were overflowing on very small screens. I implemented a FullPage plugin for this - scroll overflow: github.com/alvarotrigo/fullPage.js/blob/master/vendors/scrolloverflow.min.js.map.
    5. Embeds were problematic in that they were not re-sizing. I discovered specific embed utilities provided by Bootstrap.

## Deployment

This site was developed using Visual Studio Code and is being hosted on GitHub pages at snopp.scottymcandrew.com

To run locally all files from the Git repo are required and need to be hosted on a local web server. This can be achieved preferably with your IDE's live server feature.

## Credits

- Snoop Dogg himself! Inspiration came from his own website: snoopdogg.com/
- Behance for inspiration in building the structure of this site: www.behance.net
- Hogni for further inspiration in this site's structure: http://www.hogni.com/#home
- coolors.co for colour matching
- Google images for the image content
- W3Schools for much of the guidance, including further understanding of Flexbox, JQuery and a parallax background.

### Content

- The text for the home section was copied from the [Wikipedia article Snoop Dogg](https://en.wikipedia.org/wiki/Snoop_Dogg)
- Text for the news section was copied from Snoop Dogg's website: snoopdogg.com/news/
- The remainder of the text was written by myself but taking inspiration from Snoop Dogg's language style: www.urbandictionary.com/define.php?term=Snoop%20Dogg

### Media

- The photos used in this site were obtained from Google Images and Snoop Dogg's social media presence.
- Music was embedded from Spotify: www.spotify.com/uk/
- Videos were embedded from YouTube: www.youtube.com

### Acknowledgements

- Snoop Dogg himself! Inspiration came from his own website: snoopdogg.com/
- Behance for inspiration in building the structure of this site: www.behance.net
- Hogni for further inspiration in this site's structure: http://www.hogni.com/#home
