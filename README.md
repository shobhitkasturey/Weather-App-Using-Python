
# Basic Weather App

This is a simple weather application that fetches and displays weather data for a given location using the OpenWeatherMap API. The application also saves the recorded data to a CSV file for future reference.

## Features

- Fetch weather data for a specified location
- Display current temperature and weather conditions
- Save weather data to a CSV file
- Validate user input to ensure a valid location is provided

## Prerequisites

- Python 3.x
- `requests` library

## Installation

1. **Clone the repository:**

    ```sh
    git clone https://github.com/yourusername/weather-app.git
    cd weather-app
    ```

2. **Install the required libraries:**

    ```sh
    pip install requests
    ```

3. **Get an API key from OpenWeatherMap:**

    Sign up at [OpenWeatherMap](https://home.openweathermap.org/users/sign_up) to get a free API key.

## Usage

1. **Open the `weather_app.py` file:**

    Replace `'your_openweathermap_api_key'` with your actual API key from OpenWeatherMap.

    ```python
    api_key = 'your_openweathermap_api_key'
    ```

2. **Run the script:**

    ```sh
    python weather_app.py
    ```

3. **Enter a location:**

    When prompted, enter the name of the location for which you want to fetch the weather data.

4. **View and save weather data:**

    The weather data for the specified location will be displayed, and the data will be saved to `weather_data.csv`.

## Project Structure

weather-app/
│
├── weather_app.py # Main script for the weather application
├── weather_data.csv # CSV file to store weather data (created after running the script)
└── README.md # This README file



## Functions

### `test_weather_api(api_key, location)`
Tests the API call with the given location and prints the JSON response.

### `get_weather(api_key, location)`
Fetches the weather data for the specified location.

### `get_location()`
Prompts the user to enter a location and validates the input.

### `display_weather(data)`
Formats and displays the weather data.

### `save_weather_data(file_name, data)`
Saves the weather data to a CSV file.

## Example Output

Enter the location: London
API request successful!
JSON response:
{
"coord": {"lon": -0.1257, "lat": 51.5085},
"weather": [{"id": 800, "main": "Clear", "description": "clear sky", "icon": "01d"}],
"main": {"temp": 20.0, "feels_like": 19.0, "temp_min": 18.0, "temp_max": 22.0, "pressure": 1015, "humidity": 60},
"name": "London",
"cod": 200
}
Weather in London:
Temperature: 20.0°C
Condition: Clear sky




## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue to discuss changes.

=
