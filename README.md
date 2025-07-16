# API-INTEGRATION
COMPANY   : CODTECH IT SOLUTIONS

NAME      : R NAVYA

INTERN ID : CT08DN1419

DOMAIN    : FULL STACK WEB DEVELOPMENT

DURATION  : 8 WEEKS

MENTOR    : NEELA SANTOSH




#  Weather API Integration Webpage








This project is a dynamic and responsive web application that integrates with a **public weather API** to fetch and display real-time weather data based on user input. 




It demonstrates how to build a full-stack web solution using **Node.js**, **Express.js**, and **OpenWeatherMap API**, with a lightweight **HTML/CSS/JavaScript frontend**.




The goal of this project is to show how you can **consume external APIs** and **display data dynamically on a webpage** while ensuring security and responsiveness. 




This serves as a practical example of API integration, full-stack development, and UI design with a modern aesthetic.




The Weather API Integration Webpage is a full-stack project that demonstrates how to connect a frontend webpage to a public API using a secure backend proxy. 



It uses the OpenWeatherMap API to fetch real-time weather information for a user-entered city, and dynamically displays that data on a styled, responsive webpage.

This project consists of two main parts:


A frontend (index.html with CSS and JavaScript) where users interact and view weather data.



A backend (Node.js with Express) that securely makes API requests to OpenWeatherMap and returns results to the frontend.



## Features


- Live weather data for any city in the world
- Weather icon, description, temperature, wind speed, and humidity
- Local time of the queried city
- Responsive and mobile-friendly design
- Backend proxy server to protect the API key
- Built using clean, modular, and understandable code


  # Backend Details

  
The backend uses Express.js, a lightweight web framework for Node.js.

Axios is used for making HTTP requests to the OpenWeatherMap API.

dotenv loads the API key from the .env file, ensuring it's not hardcoded or exposed.

CORS is enabled to allow communication between frontend and backend if hosted separately.

The server is configured to statically serve the frontend folder (weather-frontend/) using express.static(), so you can open the entire application from a single URL like http://localhost:5000.

# Frontend Details

The frontend is written in HTML, CSS, and Vanilla JavaScript.

A stylish layout uses modern CSS, including glassmorphism, gradients, and mobile responsiveness.

JavaScript handles input collection, fetch calls, error handling (like city not found), and DOM updates.

The interface updates in real-time without page reloads.


## Project Structure


weather-project/

├── weather-api-backend/

     └── .env
     
     └── index.js  
     
     └── package.json
     
     └──package-lock.json
     
├── weather-frontend/


    └── index.html 
    
    └── package.json
    
    └──package-lock.json 
    
 The index.js file is the main backend entry point, which sets up an Express server, uses Axios    to make HTTP requests to the OpenWeatherMap API, and responds with JSON data.
 
 The frontend (index.html) uses plain JavaScript to request data and dynamically display it in a   stylish card.

# Technologies Used
  
Frontend: HTML5, CSS3,  JavaScript

Backend: Node.js with Express.js

API: OpenWeatherMap API

Packages: axios, cors, dotenv

Development Tools: VS Code, Node.js, npm


# Environment Setup




Before running the project, you must add your API key from OpenWeatherMap to the .env file:



WEATHER_API_KEY=your_openweathermap_api_key_here


This key will be used in the backend to authenticate requests to the weather API.

Never expose your API key in the frontend JavaScript, as it can be easily extracted from the browser.

# Working

When a user enters a city name and clicks “Get Weather”, the frontend JavaScript uses the Fetch API to call a local /weather endpoint (hosted on Express).

The server reads the city query parameter, appends it to the OpenWeatherMap URL, and sends a request using Axios.

The response, which includes weather condition, temperature, wind, and more, is then passed back to the frontend, parsed, and displayed to the user in a visually appealing layout.


# Output 

<img width="1918" height="1075" alt="Image" src="https://github.com/user-attachments/assets/e78598c6-65ea-486d-95c1-cbd9e624fe16" />


<img width="1920" height="1020" alt="Image" src="https://github.com/user-attachments/assets/81c70fc0-c805-4932-9bf6-bfa15db02362" />
