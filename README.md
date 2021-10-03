# A cleaner space, A cleaner future, MYNH CLEANER - Mapping Space Trash in real Time
 Did you know that we are at significant risk of ending all means of communication and shutting ourselves off from space? In our space there are 36500 objects greater than 10 cm, 1000000 objects from 1 cm to 10 cm and 330 million objects from 1 mm to 1 cm. The space is filled with trash pieces from the missions dispatched, and these pieces only collide to create more trash triggering a never-ending chain of space debris growth. But we have the solution, an interactive web application that provides real time location and predictions of them in real time in an interactive map providing information such as (geospatial, velocity, type, date, time) not only that but the app can predict crashing.


![logo op2](https://user-images.githubusercontent.com/75124259/135745116-e437759b-315a-4704-981e-b6213fff9994.png)



# Project Code Strategy: 

### Step 1 

1-     With the Worldwind open source we will create our 3D interactive globe to visualize the derbies surrounded Earth. We choose Worldwind as it is available for desktop, mobile, and web browser applications. We plan to use the following Code files from the library. Argument Parsing, Deep picking, Geolocation, Measurement, and Region Picking

### Step 2 

2-     In the following step we will Extract Data from NEOSSAT - Astronomy Data and Celestak. Through the following link, we will extract, clean, filter the data to extract debris and junk data. http://asc-csa.gc.ca/eng/satellites/neossat/default.asp. This dataset includes astronomical Images from closer to the earth Object surveillance satellite (NEOSSAT). As it can detect and track the asteroids and satellites at an altitude of about 780 KM above the earth. The other option is Celestak https://celestrak.com/NORAD/elements/ as a dataset for obtaining the required information to use to map the trash objects.

### Step 3 

3-     After we will obtain the required data, Python's SGP4 is a python page that can compute the exact position and velocity of the earth obtaining satellite. Hence; we can enhance the code package to fit in with our problem to map the debris. Using Python's SGP4 and the extracted data from CelesTrak or NEOSSAT - Astronomy Data, we will be able to justify the exact location for the specific debris, its longitude, latitude, and altitude.
 
 
 ### Step 4 
 
4-     Step 4 including the mapping process and displaying our results into the geospatial Wroldwind library that we use at first. Resulting we will have the following outputs as in the below photo. All the tracked debris is shown in the user interface that we will create.

![space_debris001-780x780](https://user-images.githubusercontent.com/75124259/135744446-f2c8dbdb-3d15-4528-8fcf-c9037e6cfea0.jpg)

 
 ### Step 5 
5-     In this step to achieve the goal of mapping in real-time the problem, using the same python package with adding and editing particular parameters in the code to update the time each second and display the result in the UI of our web application MYNH CLEANER.
 
 ### Step 6 
 
6-     Last step and the most important step for our solution show the added value that we bring to the problem. By using the same parameter that we extract and the resulting parameter such as time, inclination, direction, position. We will be able easily to predict if there are any debris, satellite, asteroids, and any artificial object that will collide in the future. By that, we will solve another problem which is providing expensive materials and sensors in the satellite to avoid colliding. Just with a simple code satellite will be safe. Besides, reduce and solve the major problem which is tracking the trash in Actual-time.
