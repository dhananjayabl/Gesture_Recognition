# Project Name
> Gesture Recognition


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- To develop a classifier that can accuretly classify the gestures
- There are five gesture classes:
    - Thumbs up:  Increase the volume
    - Thumbs down: Decrease the volume
    - Left swipe: 'Jump' backwards 10 seconds
    - Right swipe: 'Jump' forward 10 seconds  
    - Stop: Pause the movie
- Each video is a sequence of 30 frames 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Three types of models tested
    - 3D convolution
    - SimpleCNN with GRU/LSTM
    - Pretrained CNN with GRU/LSTM
        - InceptionV3 is used as pretrained model
- with limited experimentation as conducted above it is difficult to determine which model is best compared to other
- All 3 types of modeling has produced val accuracy > 0.9 
- It is advisable to run more experimentations and averaging the performance over multiple runs for particular model configuration
- CNN+LSTM performed better without regularization layer, where as CNN+GRU overfits and needed regularization 
- The GPU used for training is RTX2070 max-Q, large models (CNN+RNN) could not be trained, often faced OMM(out of Memory) issue, hence have to reduce the model complexity

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python 3.9.13
- Tensoflow 2.6
- Numpy 1.22.4
- OpenCV 4.5.5

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com).


## Contact
Created by [@githubusername] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
