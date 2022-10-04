# Instructions

(Fork this sandbox before getting started and please read through the full instruction below before you start coding.)

Your task in this exercise is to replicate the following UI in code: [Customized map](https://i.imgur.com/EAodRBr.png)


The app is supposed to meet the following specifications.

- Use Google maps to draw a map that covers the entire screen.
- Initially the map should be centered on times square (lat: 40.758896, lng: -73.98513)
- The Satellite button on the top right is a toggle button. Clicking on it should change the map to satellite view and the button label should change from "Satellite" to "Map". Clicking the button again should revert those changes back.
- The red location pin should stay fixed at the center of the map even as the user travels along the map by panning left and right or zooming in and out.
- Clicking the crosshair button on the bottom right should prompt the user to give his current location. (Acquire the user's location using the browser's location apis. Don't prompt the user to manually enter latitude and longitude)
- Change the map center to the acquired user location. 
- Draw a blue dot marker on the user's location.
- Draw a wider circle around the blue dot according to the gps accuracy (faded blue circle on the screenshot)


You can find the api key for working with the google maps js library defined in src/utils.ts.

# Bonus (Not required, but has extra credit)

- If you're using a third party google maps library, please remove it as a dependency. See if you can write the code for importing the google map script in React-land and handle the underlying asynchronisity.
- Can you continuously watch the user's location and update the location of the blue dot on the map according to changes in the user location?
- Similarly, can you monitor the accuracy in meters and update the accuracy circle(changing its center and radius) as the accuracy changes. 
- Can you show an alert when location access is denied.

# Evaluation criteria

- Code organization
- Appropriate use of types
- Appropriate handling of loading and error states
- Handle race conditions if any
- Quality of UX is not graded in this exercise. For instance, buttons don't have to look identical to their screenshot counterparts. Focus on functionality.
