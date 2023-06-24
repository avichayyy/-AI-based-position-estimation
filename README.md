# 046211-AI-based-position-estimation
Repository for deep learning course project - AI based position estimation based on radio frequency Project

# About
the scope of the project is cellular based UE localization for non-synchronized network power based approaches. The traditional approach(GPS) are triangulation based, those approaches rely on range estimation from known locations and it dependent on general consistent power range model. Such models is not accurate for some cases duo to Multi-Path / fading + low probability to detect more than one cell tower, localization is reduced to strongest cell or sector in the area and the error is dependent on the cell tower density.

# Dataset Collection
In our project we take data collected by RF catcher in a neighborhood in Tel-Aviv, we process the data from the machine and we try to estimate the location of the ue based on the parameters it transmitted using deep convolutional neural network.
![image](https://github.com/avichayyy/-AI-based-position-estimation/assets/129785797/a4c77950-7548-44ab-893d-8cc779b01a39)
In the picture above it is possible to see the RF catcher that was used in the process of collecting the dataset. In addition in the picture it is possible to see the routes that were traveled in Tel-Aviv while holding the RF catcher. The RF catcher transmit once a frame and this data was later processed to features that we can use for our project (WB SNR, NB CNR, CIR…). 

# Dataset Info
* The dataset contain 
In the original project the best results were achieved using decision trees. In our project we are going to try to improve the results using CNN architectures and incase it wont work we will try Fully connected approach as well.
