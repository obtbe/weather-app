# Weather App

## Introduction

The Weather App is a Java-based application that provides real-time weather information for any specified location. Users can input a location name to receive detailed weather data, including temperature, weather condition, humidity, and wind speed. This data is retrieved via an external weather API and displayed in a graphical user interface (GUI) for easy interaction. 

This document outlines the application's features, technologies, architecture, and implementation details.

## Screenshot

<p align="center">
    <img src="https://github.com/obtbe/WeatherAppGUI-Java/blob/main/Screenshot_15.png?raw=true" alt="Weather App Screenshot">
</p>

---

## Features

- Real-time weather data retrieval based on user-specified locations.
- Simple and intuitive graphical user interface.
- Weather details include:
  - Current temperature.
  - General weather conditions.
  - Humidity levels.
  - Wind speed.
- Visual weather representation with dynamically loaded icons.
- Data fetching from a reliable external weather API using geographical coordinates.

---

## Technologies Used

The Weather App leverages the following tools and libraries:

- **Java 18:** Core language for developing the application.
- **JSON Simple:** Parsing and manipulating JSON responses from APIs. Download it [here](https://code.google.com/archive/p/json-simple/downloads).
- **HttpURLConnection:** Java's built-in library for managing HTTP requests and connecting with external APIs.

---

## Class Summaries

### 1. AppLauncher

- **Purpose:** Serves as the application's entry point.
- **Functionality:** Initializes the program and launches the GUI (`WeatherAppGui`).

### 2. WeatherAppGui

- **Purpose:** Represents the application's graphical user interface.
- **Functionality:** 
  - Displays weather information retrieved from the API.
  - Includes UI components like text fields, labels, and images.
  - Handles user interaction for searching and displaying weather details.

### 3. WeatherApp

- **Purpose:** Manages the backend logic, including fetching and processing data from the weather API.
- **Key Responsibilities:** 
  - Retrieve geographical coordinates based on location names.
  - Fetch hourly weather data for the current time and location.
  - Convert raw weather codes into user-friendly descriptions.
  - Provide methods to parse API responses and format time for better accuracy.

---

## Setup Instructions

### Prerequisites

- Java Development Kit (JDK) 18 or later installed.
- JSON Simple library added to your project's build path.

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/obtbe/WeatherAppGUI-Java.git
    ```
2. Open the project in your favorite IDE (e.g., IntelliJ, Eclipse).
3. Add the `json-simple` library to the project's dependencies.
4. Run `AppLauncher.java` to start the application.

### Asset Integration

Ensure the `assets` folder with weather icons (e.g., cloudy, rainy, sunny) exists under `src/assets` in your project directory. This enables dynamic visual updates based on the weather condition.

---

## Example Workflow

1. Launch the application.
2. Enter a location in the search field.
3. View current weather details, including:
   - Temperature.
   - Weather condition (with an image).
   - Humidity percentage.
   - Wind speed.

---

## Contributing

Feel free to fork the repository and submit pull requests to contribute to the Weather App. Bug reports and feature requests are also welcome via the [issues page](https://github.com/obtbe/WeatherAppGUI-Java/issues).

---


