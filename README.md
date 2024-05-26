# Mapty

Mapty is a workout tracking application that allows users to log their running or cycling workouts on a map. The application displays detailed information about each workout, such as distance, duration, cadence, and elevation, and stores the workout data in the browser's local storage for persistence.

## Features

1. **Workout Logging**:
   - Users can log workouts (running or cycling) on a map.
   - The form captures workout details such as distance, duration, cadence (for running), and elevation (for cycling).
   - A map marker is added at the workout location with a popup displaying the workout type and date.
   - The sidebar shows a list of workouts with detailed information.

2. **Geolocation**:
   - The app uses the Geolocation API to get the user's current position and load the map centered on that location.

3. **Map Interaction**:
   - Users can click anywhere on the map to open the workout form.
   - Clicking on a workout in the sidebar moves the map to the corresponding workout marker.

4. **Local Storage**:
   - All workout data is stored in the browser's local storage.
   - Workout data is loaded from local storage when the application starts, ensuring persistence across sessions.

## Project Details

### Development Insights

This project was developed with insights from Jonas Schmedtmann's "The Complete JavaScript Course". The HTML and CSS starter files were provided by Jonas, and the Leaflet library was explored to implement map functionalities and the Geolocation API.

### Object-Oriented Programming

The project utilizes JavaScript's Object-Oriented Programming (OOP) features. The main application architecture is encapsulated in an `App` class, which manages the overall functionality. Additionally, the project includes the following classes:

- **Workout Class**: Contains common properties and methods for all workout types.
- **Running Class**: Extends the `Workout` class, adding specific properties and methods for running workouts.
- **Cycling Class**: Extends the `Workout` class, adding specific properties and methods for cycling workouts.

### How It Works

1. **Initialization**:
   - The app gets the user's position and loads the map centered on that location.
   - Workout data is loaded from local storage and rendered on the map and sidebar.

2. **Logging a Workout**:
   - Users click on the map to open the workout form.
   - Users fill out the form with workout details and submit it.
   - A workout object is created based on user input and added to the workout array.
   - The workout is rendered on the map as a marker and in the sidebar as a list item.
   - Workout data is saved to local storage.

3. **Navigating to Workouts**:
   - Users can click on a workout in the sidebar to move the map to the corresponding workout marker.

## Technologies Used

- **JavaScript**: Core programming language used for implementing the application logic.
- **HTML/CSS**: Provided by Jonas Schmedtmann as starter files for the project.
- **Leaflet**: Open-source JavaScript library used for interactive maps.
- **Geolocation API**: Used to get the user's current position.
- **Local Storage**: Web API used for storing workout data persistently in the browser.

## Demo

You can view a live demo of the Mapty application [here](https://jay31kr.github.io/mapty/).

## Author

Created by [Jay](https://github.com/Jay31kr). Click the link to visit my GitHub profile.
