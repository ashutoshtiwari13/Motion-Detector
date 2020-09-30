![](https://img.shields.io/badge/Made%20with%20%3C3%20in-python-red.svg)

# Motion- Detector System Using OpenCV 
Python/OpenCV scripts that detect motion on webcam and allow record it to a file and plot a graph for proper Visualization.

## Description 

### The Process 

The trivial idea is to compute the difference between two frames apply a threshold the separate pixels that have changed from the others and then count all the black pixels. Then the average is calculated with this count and the total number of pixels and depending of the ceil the event is triggered or not.

#### Additional informations: 
* initRecorder - initialise the recorder with an arbitrary codec it can be changed with problems
in the run method no motion can be detected in the first 5 second because it is almost the time needed for the webcam to adjust the focus and the luminosity which imply lot's of changes on the image
* processImage - contains all the images operations applied to the image
* somethingHasMoved - The image iteration to count black pixels is contained in this method

## Requirements

* X86, X86_64, ARMv7 or ARMv8 version of Ubuntu 18.04 or Debian 8 (will most likely work on other Linux based operating systems as well)
* Python 3.5 or above 
* Camera or Video file
* [Install OpenCV](https://opencv.org/) or `pip install opencv-python`
* [Install Bokeh library](https://bokeh.pydata.org/en/latest/) or `pip install bokeh`

## Run Motion Detecto5
Clone the repository and run the command `python plotting.py` in the project directory.

#### Scenario 1

![alt text](https://github.com/ashutoshtiwari13/Motion-Detector/blob/master/SS1.png)

#### Scenario 2(Under motion) 

![alt text](https://github.com/ashutoshtiwari13/Motion-Detector/blob/master/SS2.png)

## Result 

![alt text](https://github.com/ashutoshtiwari13/Motion-Detector/blob/master/SS3.png)

## Plotting
![alt text](https://github.com/ashutoshtiwari13/Motion-Detector/blob/master/SS4.png)

## Use case & Future Scope 
* Motion Detector can be used on SBCs such as Raspberry Pi, NanoPi M1, CHIP, ODROID C1/C2/XU4, Pine A64, etc. to create compact smart cameras. 
* Threading and subprocess based architecture allows consistent FPS while processing frames, writing video files, moving files to remote location, etc. all concurrently.
* Run multiple copies on a central server for IP based "dumb" cameras.
* Supports several types of video inputs including USB and IP (wired/wireless) cameras, video files, etc.
* Threshold based motion detection, ignore mask, multiple object marking and video recording.
 * Human feature detection with the ability to train your own detector.
* Add your own plugins.

Help me with a :star: if you like my work. :bowtie:
happy Coding ! :heart:
