# tidal-bulge-model

This repository shows the movement of simulated tidal bulges and analemma across the Earth's surface over a single day and over 365 days in 2023. It aims to spatially show the relation between the position of the Moon and Sun relative to Earth and the resulting net force enacted on the surface.

Animation previews, as they will likely need to be downloaded: 

- 2023-tidal-bulge-and-analemma.mp4:

<img width="925" alt="Screenshot 2024-08-16 at 11 18 04 AM" src="https://github.com/user-attachments/assets/6ccf7095-8750-490a-bc5c-88a230c52790">


- April-5-2023-tidal-bulge.mp4:

<img width="924" alt="Screenshot 2024-08-16 at 11 17 41 AM" src="https://github.com/user-attachments/assets/f0bc9121-c5e7-4813-a1a4-9e927ed7669b">


In the tidal bulge model, the combined gravitational forces of the Sun and Moon on the Earth's surface drive the creation of tidal "bulges," areas with high and low water levels. Areas experiencing high net force, when the Sun and Moon are approximately aligned, observe a "spring tide," while areas experiencing low net force, when the Sun and Moon are at approximately 90 degree angles, observe a "neap tide." 

<img width="276" alt="image" src="https://github.com/user-attachments/assets/36a3f870-ab16-4f36-8552-b3fc36d45cc7">

- Source: https://science.nasa.gov/moon/tides/


The tides in reality are influenced by myriad other factors, including the presence and shape of land masses (e.g. the continents), the ocean's bathymetry, and wind. 

The analemma is a figure-8 shape that occurs when tracking the location of the Sun at the same time each day for a full year. The vertical up-and-down motion results from the Earth's axial tilt (also the cause of the seasons), while the horizontal back-and-forth results from Earth's orbital eccentricity (elliptical shape). 

<img width="935" alt="Screenshot 2024-08-16 at 11 03 59 AM" src="https://github.com/user-attachments/assets/eece9d0d-8128-42ac-a648-9bb53d7c5272">

- Source: https://www.skymarvels.com/infopages/vids/Earth%20-%20DayNight%20001.htm


<img width="408" alt="image" src="https://github.com/user-attachments/assets/679582c6-281d-4573-9d2c-f527d3d4ff3e">

- Source: https://oceanservice.noaa.gov/education/tutorial_tides/tides03_gravity.html 

This project determines the relative locations of the Sun and Moon for an arbitrary date and time (24 hours on April 5, 2023 and midnight each day for the full year of 2023 were used for the uploaded animations), and then calculates the following vectors for a grid of points on the Earth's surface: 
- Moon's gravity exerted on the Earth's surface
- Sun's gravity exerted on the Earth's surface
- Centrifugal force from the Earth-Moon system
- Centrifugal force from the Earth-Sun system
- In addition, it also calculates the angle between the Sun and Moon.

Diagrams of the forces and directions involved, all from https://www.cambridge.org/us/files/1913/6681/8626/7708_Tidal_distortion.pdf

- Centrifugal force: 
<img width="414" alt="image" src="https://github.com/user-attachments/assets/5a8fc8e0-3be6-45e4-b6c8-aa265a0878e0">

- Resulting net force from centrifugal and gravitational forces: 
<img width="326" alt="image" src="https://github.com/user-attachments/assets/1dd18a3c-3b55-43e8-977f-b1accec42f10">

Known issues:
- does not account for tidal lag, in which the tidal bulge is approximately 50 minutes offset from the Moon's passage overhead, rather than directly aligned with it.
![image](https://github.com/user-attachments/assets/a163eac4-40b3-427e-bd3b-109698946d3d)
- source: https://science.nasa.gov/moon/tides/

Youtube link: https://www.youtube.com/watch?v=eADuR4ZpXUU
