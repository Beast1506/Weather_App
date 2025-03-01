# Weather Forecast App

[![Streamlit App](https://img.shields.io/badge/Streamlit-App-blueviolet)](https://streamlit.io/)
[![Python](https://img.shields.io/badge/Python-3.x-blue)](https://www.python.org/)

This is a simple web application built with Streamlit for displaying current weather information and making predictions for the next 3 days based on historical weather data.

**https://weatherappforecast.streamlit.app/**

## Features

* **Current Weather Display:** Fetches and displays current weather information from OpenWeatherMap, including temperature, weather condition, humidity, pressure, visibility, and wind speed/direction for a specified city.
* **Historical Weather Data:** Retrieves historical weather data using the Visual Crossing Weather API to train predictive models.
* **Predictions:** Utilizes machine learning (Random Forest Regressor) to predict the maximum and minimum temperatures for the next 3 days based on historical data.
* **Interactive Map:** Shows the location of the specified city on an interactive map with a marker indicating the current temperature.
* **Error Handling:** Manages invalid city names and API key issues.

## Technologies Used

* Streamlit: For building the web application interface.
* Requests: For making HTTP requests to fetch weather data from APIs.
* Pandas: For data manipulation and analysis.
* Scikit-learn: For implementing the Random Forest Regressor model.
* Folium: For creating interactive maps within the application.

## How to Use

1.  Clone this repository: `git clone https://github.com/Beast1506/Weather_App.git`
2.  Navigate to the project directory: `cd Weather_App`
3.  Create a virtual environment (recommended): `python -m venv venv`
4.  Activate the virtual environment:
    * On Windows: `venv\Scripts\activate`
    * On macOS/Linux: `source venv/bin/activate`
5.  Install the required dependencies: `pip install -r requirements.txt`
6.  Ensure you have your OpenWeatherMap and Visual Crossing Weather API keys stored as environment variables.
7.  Run the Streamlit app: `streamlit run app.py`
8.  Enter the name of the city for which you want to fetch weather information in the app.
9.  Click on "Show Current Weather" to display the current weather details.
10. Click on "Predictions For Next 3 Days" to view weather predictions for the next 3 days.
11. Click on "Show Weather Map" to visualize the location of the city on the map with the current temperature marker.

## API Keys

* You will need API keys from:
    * OpenWeatherMap
    * Visual Crossing Weather
* Please store these keys as environment variables for security.

## Contributing

Feel free to contribute or provide feedback to improve the app!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.txt) file for details.
