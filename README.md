# Primephonic iOS coding challenge
Thanks for your interest in Primephonic and for taking the time to do our iOS coding challenge. We hope you enjoy developing it as much as we did :)

## Task
Your task is to write an iOS application which displays some basic information of flights currently in the air. For this, we'll be using the `OpenSky Network` public API:

- API Documentation can be found here: `https://opensky-network.org/apidoc/rest.html`
- Only the following endpoint should be used: `GET /states/all`

The application should be made up of 2 screens:

### 1. Map Screen
This screen should display a map view of the entire world, centered on the device's `current location`. This view should be populated with all of the aircrafts returned by the API (one marker per aircraft), and should be refreshed automatically every 10 seconds.

On every update, the map only needs to display the updated data (no animation required between previous position and current position of aircrafts). However, the application should keep track of the history of updates received throughout time, as it will be used in the next part of the assignment.

Upon tapping on one specific marker/aircraft, the application should take the user to the next screen.

### 2. Details Screen
This screen should display the history of updates for this particular aircraft, from newest (latest position update for this aircraft) to oldest (first position update received for this aircraft). The UI of this screen is entirely up to you.

## Evaluation criteria
The assignment will be evaluated based on the following points:

1. Code organization
<br/>Is the code well organized, easy to follow, well-structured, etc.? Think responsibilities, separation of concerns.

2. Performance
<br/>The API might return a single aircraft, or thousands. Your application should be able to handle all scenarios seamlessly.

3. Compliance
<br/>Does the application satisfy the described use cases?

4. Simplicity
<br/>Don't over-engineer it. If you feel like you're taking shortcuts you're not comfortable with, go with the simple solution and later explain how you would do it differently in a real production app in the `README.md`.

## Technologies
The assignment should be developed in `Swift`. Third party libraries are allowed.

## Submission Guidelines
- Submit your project in a single `zip` file to your Primephonic contact.
- Include a `README.md` with instructions on how to run it, together with any additional information you consider appropriate (assumptions, design decisions made, etc.)
- Include *only* source code and assets (no libraries, modules, etc.)
