# Weather App

This is a simple JavaScript Weather App that fetches weather data from the [OpenWeatherMap API](https://openweathermap.org/) and displays it in a user-friendly interface.

## Features

- Displays the current weather for a specific location.
- Shows temperature, weather condition, humidity.
- User can search for weather by city name.
- Supports multiple units Celsius.
- Responsive design for mobile and desktop views.

## Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [Technologies Used](#technologies-used)
- [Usage](#usage)
- [API](#api)
- [Contributing](#contributing)
- [License](#license)

## Installation

### Prerequisites
- A code editor like [VS Code](https://code.visualstudio.com/)
- Basic knowledge of HTML, CSS, and JavaScript
- A valid OpenWeatherMap API key

### Steps to install
1. Clone this repository:
    ```bash
    git clone https://github.com/Smyekh/Weather-APP.git
    cd Weather-APP
    ```

2. Install dependencies (if any):
    ```bash
    npm install
    ```

3. Get your API key from [OpenWeatherMap](https://home.openweathermap.org/users/sign_up) by signing up for a free account.

4. Create a `.env` file in the root directory and add your API key:
    ```bash
    API_KEY=your_openweathermap_api_key
    ```

5. Open `index.html` in your browser to run the app.

## Technologies Used

- **HTML5**: Structure the webpage.
- **CSS3**: Styling for layout and design.
- **JavaScript (ES6+)**: Handles API calls and DOM manipulation.
- **Fetch API**: To make HTTP requests to the OpenWeatherMap API.
- **OpenWeatherMap API**: Source of weather data.

## Usage

1. Open the application in your browser.
2. Enter a city name in the search bar to get the current weather.
3. Optionally toggle between Celsius and Fahrenheit.

## API

This app uses the [OpenWeatherMap API](https://openweathermap.org/api) to fetch weather data. You need an API key to access the data.

### API Endpoint Example
**Current Weather Data by City:**

`GET https://api.openweathermap.org/data/2.5/weather?q={city_name}&appid={API_key}`

### Query Parameters
- `q`: City name (required)
- `appid`: Your API key (required)
- `units`: Units of measurement (optional, "metric" for Celsius, "imperial" for Fahrenheit)

### Example Response
```json
{
  "main": {
    "temp": 15.0,
    "humidity": 80
  },
  "weather": [
    {
      "description": "clear sky",
      "icon": "01d"
    }
  ],
 
```

## Contributing

1. Fork the repository.
2. Create your feature branch:
   ```bash
   git checkout -b feature/new-feature
   ```
3. Commit your changes:
   ```bash
   git commit -m 'Add some feature'
   ```
4. Push to the branch:
   ```bash
   git push origin feature/new-feature
   ```
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
