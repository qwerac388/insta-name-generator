# Insta Name Generator

The Insta Name Generator is a simple, web-based application that helps users generate random Instagram usernames. The application is built on Node.js and Express, utilizing EJS for templating. For seamless deployment and accessibility, the application is hosted on Heroku.

## Features

- Random Username Generation: Combines an adjective and a noun to create a unique Instagram name.
- Simple Web Interface: A user-friendly interface with a welcoming message and a single button to generate the name.
- Adaptive Layout: The application's design is made responsive with CSS, ensuring compatibility and an optimized viewing experience across different devices.
- Heroku Deployment: The application is deployed on Heroku, enabling easy access and high availability.

## Preview

When a user visits the website, they are greeted with a message "Welcome to the Insta Name Generator" and a "Generate Name" button.

![Preview of the Insta Name Generator](public/styles/Preview1.gif)

---

Upon clicking the button, the server generates a random combination of an adjective and a noun, which is then displayed to the user as a suggested Instagram name.

![Preview 2 of the Insta Name Generator](public/styles/Preview2.gif)

## Live Application

The Insta Name Generator is now live! Check it out here: [Insta Name Generator](https://insta-name-generator-2bd08e87d766.herokuapp.com/)

## Technical Details

index.ejs

- The main page of the application, which includes the templating logic to display the generated Instagram name or a welcome message if no name has been generated yet. It also includes a form that posts to the /submit endpoint to trigger the generation of a new name.

index.js (Server)

- The server-side JavaScript file powered by Node.js and Express. It handles routing, name generation, and the serving of static files.

Key Components:

- Express App: Sets up a server to handle incoming HTTP requests.
- Middleware: Uses body-parser for form submission handling and serves static files from the public directory.
  Routing:
- GET /: Renders the index.ejs file.
- POST /submit: Handles the generation of the new Instagram name using arrays of adjectives and nouns.
- Port Configuration: Configured to work with both Heroku deployment and local development environments.

## Installation and Running the App

To run the Insta Name Generator, Node.js must be installed on the system. Following that, these steps will get the app up and running:

- Clone the repository to your local machine.
- Navigate to the cloned directory.
- Install the dependencies using npm install / npm i.
- Start the application with nodemon index.js.
- Open a web browser and go to http://localhost:3000 to view the app.

## Contributing

Contributions are welcome! If you have suggestions or want to improve the app, feel free to make a pull request or open an issue.
