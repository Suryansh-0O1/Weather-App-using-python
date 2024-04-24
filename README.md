# Weather-App-using-python
This is a Python script that creates a graphical user interface (GUI) for a weather application using the Tkinter library. Here's a breakdown of the code:

# Importing libraries

The script starts by importing several libraries:

- requests: for making HTTP requests to the OpenWeatherMap API
- tkinter (and its submodules messagebox and Image): for creating the GUI
- datetime: for working with dates and times
- configparser: for reading configuration files
- os: for interacting with the operating system

# Configuring the GUI

The script creates a Tk object, which is the main window of the GUI, and sets its title, background color, and geometry.

# Reading configuration file

The script reads a configuration file named config.ini using the ConfigParser library. The configuration file contains an API key for the OpenWeatherMap API.

# Defining functions

The script defines three functions:

- get_weather(): retrieves the current weather data for a given city from the OpenWeatherMap API and updates the GUI with the data.

- reset(): resets the GUI to its initial state by clearing all input fields and labels.

- get_forecast(): retrieves the weather forecast for a given city from the WTTR.in API and prints the response to the console.

# Creating GUI elements
The script creates several GUI elements, including:

- Labels: for displaying text, such as the title, city input label, and weather data labels
- Buttons: for submitting the city input, getting the weather forecast, and resetting the GUI
- Entry fields: for inputting the city name and displaying the weather data
- A timelabel element: for displaying the current date and time

# Layout
The script uses the grid method to arrange the GUI elements in a grid layout.

# Main loop
The script starts the GUI event loop using the mainloop method, which runs the GUI until it is closed by the user.

# Functionality

Here's how the GUI works:

- The user inputs a city name in the city_input field and clicks the "Get Weather" button.
- The get_weather function is called, which retrieves the current weather data for the input city from the OpenWeatherMap API.
- The function updates the GUI with the weather data, including the temperature, pressure, humidity, wind speed, cloudiness, and description.
- The user can click the "Weather Forecast" button to retrieve the weather forecast for the input city from the WTTR.in API.
- The user can click the "Reset" button to clear all input fields and labels and reset the GUI to its initial state.
