# Pedi Peri-LED angle calculator (manual 3d reconstruction)

A simple piece of code I have written to find angles, that LED's subtent from the center of the dome.

## About

Perimetry plays an important role in diagnosing visual path way disorders. A variety of perimeters are available for clinical testing in adults, however no such device exists for infants.

For this a hemispherical dome (embedded with LEDs) was constructed with steel rods.The dome was covered with a black cloth. Twenty four meridians separated by 15 degrees formed the skeleton of the dome. An infrared camera was placed at the apex of the dome to capture the eye or head movement of the children during the test.

This project was done by me as part of my internship at LV Prasad Eye Institute in Srujana Center for Innovation

###### Read more [here](https://theophthalmologist.com/issues/0616/the-diagnostic-dome/)

![pedi peri](https://cloud.githubusercontent.com/assets/17895582/24576643/57b7137e-16dd-11e7-8477-ffb1ee62e803.jpg)

Due to some manufacturing practices the are some minor defects in the LED's positioning. To exactly know where baby is gazing we need to map this LED's posotion with respect to  camera's position.

To do this. each and meridian was sketched on to a sheet and later we scanned the sheet to get a soft copy. 

![sandeep](https://cloud.githubusercontent.com/assets/17895582/24576707/8ef96318-16de-11e7-96b9-736ccf895bf9.jpg)


Usind solidworks a 3D model has been re-constructed from the soft copy by doing a 3d sktech.


![eee](https://cloud.githubusercontent.com/assets/17895582/24576740/5e9c603e-16df-11e7-8945-25dd9b38de6e.PNG)

Solidworks gives X Y Z coordinates of all points from the sketch on a CSV file. By using this I have to find the angles that each LED subtent at the center to know the exact posotion where baby is looking.

## How the code works

I used python to execute the program. 

 * The camera position was taken as the point of eferenceand made it orgin by subtracting it's values from all the X Y Z values.
 * Then the code first reads the data file. 
 * Columns are assigned with names.
 * Here basic pythogaros formual is implemented to all values to find the angles.
 * The values are then writen to a new CSV file.




This might not be the best method to do this. But this was just a start for me into programming.
