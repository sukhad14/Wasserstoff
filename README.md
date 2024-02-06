#WASSERSTOFF FRONTEND DEV ASSIGNMENT

### Problem Statement: [https://www.figma.com/file/ppNMpYAmwAxgSTvbr1wLmC/Wasseerstoff-Front-end-Developer-Task?type=design&mode=design]
### Hosted Website link: [https://wasserstoffreact.netlify.app]
### git repo link: [https://github.com/sukhad14/wasserstoff]
### Video demonstration link: [https://drive.google.com/file/d/17BYvlT0K-F-kKCPz5bnRMZ4MG-cYHMO6/view?usp=drive_link]

## Technical Stack/Libraries Used:

  1. React JS - Javascript based frontend library, specially used for creating SPA's.

  2. Chart.JS  -   Javascript based library which is used to display data in different forms charts.

  3. React Loader Spinner - Javascript library which has wide variety of pre-built loader animation.

  4. React router dom - Router library which is used to navigation routes in our react acpp.

  5. Styled Components 

  6. HTML, CSS


## Steps to run the project:

  1. Make sure node js is installed in your system and also has environment build path setup for node js.

      Download Nodes: [https://nodejs.org/en]

  2. Clone the repository from https://github.com/sukhad14/wasserstoff.git using command:

      ## #git clone 

  3. One the project directory in vs code.

  4. One the vs terminal at the root directory of project.

  5. Install the node modules using npm:

      ## #npm i

  6. Once the node modules finish downloading, run npm start command.

       ## #npm start

  7. Wait for localhost get hosted. [Default localhost port is 3000] 


## Approach I tried and went while developing the project:

 While reviewing the figma of the requirement, I immediately encountered the challenge of implementing a hexa world map, which I had never done before. It was a new task for me, especially since it was explicitly stated that we had to implement everything using code. Initially, I considered using svg code directly, but I wanted to understand the actual implementation process. I extensively searched online and came across some map libraries. I started exploring these libraries and learned about rendering maps using geopoints or x y coordinates. Interestingly, even the library I found internally used svg. Therefore, I realized that the first step was to obtain the geoJson of the world. Although the library provided good support for a simple map, it didn't offer any assistance for a hexabin map. I found an example for a hexabin map of the US, but it only provided x and y coordinates, not the geoJson. I attempted to find x and y coordinates for the hexabin of the entire world, but unfortunately, I could only find them for the US region. I then tried to generate my own hexabins by dividing the world map into smaller hexabins, but this approach also failed. As a result, I decided to extract the path from an svg and use it in the d3js library, but this attempt was also unsuccessful. Finally, I decided to prioritize other views and leave the hexabin map for later. 

There seemed to be a communication gap in the requirements, as there were three screens to be developed, but all the screens were directed to the overview page in the navigation route. To address this, I assigned one screen to a different route, specifically for analytics. 

The next challenge was to implement a bar chart, for which I started using the d3js library. I was successful in implementing it, but unfortunately, I encountered occasional errors for which I couldn't find much support online. Consequently, I manually created the bar chart and completed the overview page without the hexabin map. I then proceeded to the second page, where I had to develop a bubble chart. This chart involved bubbles of different sizes, colors, and shadows. I attempted to create a single component for both texted and non-texted bubbles using #.