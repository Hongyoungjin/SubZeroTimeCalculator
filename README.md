# 1. SubZeroTimeCalculator
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

# 2. GraspPointFinder
Based on the "Force Closure" idea, the algorithm intends to find the optimum grasp point of a virtual 3D object.


## How it works
1. Import 3D object (stl or obj file)
2. Find possible grasp points (center of each mesh) and their wrench values in the matrix form
3. Make GWS (grasp wrench space)
4. Find the best grasp (grasp of the largest grasp quality)


## Brief explanation of each code
1. "gws_to_cone.py" : 
- From 3D object, makes GWS data, and 3D object attached with friction cones of all possible grasp points
2. "searchall.py"   : 
- Finds the best grasp among all possible grasp candidates - Most accurate, yet takes too much time
3. "gpsearch.py"    : 
- Finds the locally best grasp through regressively updating the grasp  - Quicker, yet less accurate (80% accurray on average)

## How to execute
### If you want to find the accurate data taking a lot of time
1. gws_to_cone.py
2. searchall.py

### If you want to find the less accurate data within short period of time
1. gws_to_cone.py
2. gpsearch.py
