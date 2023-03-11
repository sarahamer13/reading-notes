## In today's reading we learn how to add pictures and videos to the page ##


### *Explain how the ability to use video and audio on the web has evolved since the early 2000s* ###

- The first influx of online videos and audio were made possible by proprietary plugin-based technologies like Flash and Silverlight. Both of these had security and accessibility issues, and are now obsolete, in favor of native HTML solutions < video > and < audio > elements and the availability of JavaScript APIs for controlling them. We'll not be looking at JavaScript here — just the basic foundations that can be achieved with HTML.


### *Describe the use of the src and controls attributes in the < video > element* ###

- The < video > element allows you to embed a video very easily.

- In the same way as for the < img > element, the src (source) attribute contains a path to the video you want to embed. It works in exactly the same way.

- Users must be able to control video and audio playback (it's especially critical for people who have epilepsy.) You must either use the controls attribute to include the browser's own control interface, or build your interface using the appropriate JavaScript API. At a minimum, the interface must include a way to start and stop the media, and to adjust the volume.

### *Why is it important to have fallback content inside the < video > element?* ###

- The paragraph inside the < video > tags
This is called fallback content — this will be displayed if the browser accessing the page doesn't support the < video > element, allowing us to provide a fallback for older browsers. This can be anything you like; in this case, we've provided a direct link to the video file, so the user can at least access it some way regardless of what browser they are using.

### *How does Grid layout differ from Flex?* ###

- CSS Grid Layout (aka “Grid” or “CSS Grid”), is a two-dimensional grid-based layout system that, compared to any web layout system of the past, completely changes the way we design user interfaces. CSS has always been used to layout our web pages, but it’s never done a very good job of it. First, we used tables, then floats, positioning and inline-block, but all of these methods were essentially hacks and left out a lot of important functionality (vertical centering, for instance). Flexbox is also a very great layout tool, but its one-directional flow has different use cases — and they actually work together quite well.

### *Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences* ###

- Grid Container the element on which display: grid is applied. It’s the direct parent of all the grid items.

- Grid Item the children (i.e. direct descendants) of the grid container. Here the item elements are grid items, but sub-item isn’t.

- Grid Line the dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column. Here the yellow line is an example of a column grid line.

### *Besides making a site visually appealing across different screen sizes, why should developers make images responsive?* ###

- An improvement would be to display a cropped version of the image which displays the important details of the image when the site is viewed on a narrow screen. A second cropped image could be displayed for a medium-width screen device, like a tablet. The general problem whereby you want to serve different cropped images in that way, for various layouts, is commonly known as the art direction problem

### *Define the following < img > attributes srcset and sizes. Write an example of how they are used* ###

- The standard < img > element traditionally only lets you point the browser to a single source file

- Srcset defines the set of images we will allow the browser to choose between, and what size each image is. Each set of image information is separated from the previous one by a comma

- Sizes defines a set of media conditions (e.g. screen widths) and indicates what image size would be best to choose, when certain media conditions are true — these are the hints we talked about earlier

### *How is srcset more helpful for responsive images than CSS or JavaScript?* ###

- The srcset and sizes attributes look complicated, but they're not too hard to understand if you know how to format them, with a different part of the attribute value on each line. Each value contains a comma-separated list, and each part of those lists is made up of three sub-parts

(Reference: Developer Mozilla and CSS Tricks Website)

## Things I want to know more about 

- None for now