# Weather-Tracker
A website that returns the current and 5-day weather forecast for any city that you search for, powered by Open Weather Map's API.

Through the use of Open Weather Map, this application will provide current forecast, 5-day forecast, and UV index, through 3 separate calls to the API. Five-day forecast and UV index utilize the coordinates provided in the call to the current forecast API - thus, the calls to former are nested within the call to the latter.

Upon entering a city name and clicking the search bar, the page populates with pertinent weather data, including temperature, humidity, wind speed, etc. If the city name does not exist, the search will not be called. In addition, the name of the city will be added to the left-hand side of the screen in the history tab, creating its own button. Clicking this button will reload the weather data for that specific city.


*KNOWN ISSUES*
-Within the history button field, clicking the most recently created button will not trigger the weather to populate for that city - it will only do so if it then changes from being the most recently searched city.
-JSON.parse() is incorrectly parsing local storage for the search history buttons; as such, local storage is not currently functioning.
