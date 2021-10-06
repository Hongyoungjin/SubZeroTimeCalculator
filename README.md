# SubZeroTimeCalculator
Designed to calculate the total hours of sub-zero temperature of the region in interest.


## How it works
1. Crawls the hourly temperature data
2. Selects the one that is subzero
3. Converts them to number of heater switch activation


## Click the image to watch the video
[![Video Label](http://img.youtube.com/vi/rOdQ9U1Fknk/0.jpg)](https://youtu.be/rOdQ9U1Fknk=0s)

## Brief explanation of each code
1. "Korea_Requests_Jupiter.ipynb" : 
- Using "requests" module, the code collects hourly weather data of South Korea, processes the data into the switch's annual operation rate
2. "Korea_Selenium_Jupiter.ipynb"   : 
- Using "Selenium" module, the code collects hourly weather data of South Korea, processes the data into the switch's annual operation rate
3. "WeatherWorldwide.ipynb"    : 
- Using "Selenium" module, the code collects hourly weather data of the any location globally, processes the data into the switch's annual operation rate

