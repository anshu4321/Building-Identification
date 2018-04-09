# Building-Identification
The goal is to identify buildings from satellite images. We are going to generate the images by using the google maps API, this will give us the satellite image as well as the street view of the image. 


![alt text](https://github.com/anshu4321/Building-Identification/blob/master/Images/Screen%20Shot%202018-04-09%20at%206.21.49%20AM.png)

The GetStreetImage and GetSatImage function has four inputs - latitude, longitude,resolution of your image and the range of your image. 
They get the satellite image and the street view of a certain location based on the latitude and longitude of your input.

![alt text](https://github.com/anshu4321/Building-Identification/blob/master/Images/Screen%20Shot%202018-04-09%20at%206.43.07%20AM.png)

![alt text](https://github.com/anshu4321/Building-Identification/blob/master/Images/Screen%20Shot%202018-04-09%20at%206.46.22%20AM.png)

A building is represented by gray pixels within street view, we are going to binarize the street view and place it on top of the
satellite image. 

![alt text](https://github.com/anshu4321/Building-Identification/blob/master/Images/Screen%20Shot%202018-04-09%20at%207.26.26%20AM.png)

The street view images are processed so that only the buildings which are represented by gray in the street view remain.The image
is then binarized and color negated so that the buildings which were represented by white, and all the other components of the image
are represented by black.

![alt text](https://github.com/anshu4321/Building-Identification/blob/master/Images/Screen%20Shot%202018-04-09%20at%207.41.36%20AM.png)

