# 046211-AI-based-position-estimation
Repository for deep learning course project - AI based position estimation based on radio frequency Project

# About
the scope of the project is cellular based UE localization for non-synchronized network power based approaches. The traditional approach(GPS) are triangulation based, those approaches rely on range estimation from known locations and it dependent on general consistent power range model. Such models is not accurate for some cases duo to Multi-Path / fading + low probability to detect more than one cell tower, localization is reduced to strongest cell or sector in the area and the error is dependent on the cell tower density. In the original project the best results were achieved using decision trees. In our project we are going to try to improve the results using CNN architectures.

# Dataset Collection
In our project we take data collected by RF catcher in a neighborhood in Tel-Aviv, we process the data from the machine and we try to estimate the location of the ue based on the parameters it transmitted using deep convolutional neural network.
![image](https://github.com/avichayyy/-AI-based-position-estimation/assets/129785797/a4c77950-7548-44ab-893d-8cc779b01a39)
In the picture above it is possible to see the RF catcher that was used in the process of collecting the dataset. In addition in the picture it is possible to see the routes that were traveled in Tel-Aviv while holding the RF catcher. The RF catcher transmit once a frame and this data was later processed to features that we can use for our project (WB SNR, NB CNR, CIR…). 

# Dataset statistics 
Features histogram:
![image](https://github.com/avichayyy/-AI-based-position-estimation/assets/129785797/bdd48c5b-fe40-41de-907e-fa5b7d316b59)

Number of activations for each feature:

![image](https://github.com/avichayyy/-AI-based-position-estimation/assets/129785797/f535a118-aed2-4dbc-bbd6-82e550700b41)

* Number of samples: 36,119
* Number of feature: 96
* train / test split: 85% / 15%

# Proposed CNN model
we wanted the model to be simple, yet accurate, and genaralizable enough to be able predict the location as good as we can get with the dataset:
 -- picture --
 Total of 8 convolution layers and 3 fully connected layers.

 # Results comparing
 ![image](https://github.com/avichayyy/-AI-based-position-estimation/assets/129785797/2258e7a9-4ff4-4574-933b-37a371ac18d1)

