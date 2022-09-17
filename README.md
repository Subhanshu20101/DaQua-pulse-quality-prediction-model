# DaQua-pulse-quality-prediction-model

This is an automated smartphone-based pulse grain quality anaylsis using physical dimensions.

## About the project

![alt text](https://github.com/Subhanshu20101/DaQua-pulse-quality-prediction-model/blob/main/Images/architecture.png)
In this project, we propose a smart technique for pulse quality analysis called DaQua. The proposed method employs image processing combined with machine learning to automatically segment the Region of Interest (ROI) and extract features for categorization. The smartphone’s camera acts as a sensor, capturing the image of the pulse grain, determining physical properties in real-world dimensions and using machine learning algorithms to determine the pulse sample’s quality.The user must take a picture of a small amount of pulse, and the application will analyse it and provide the necessary information.

## Features

* It uses smartphone as a sensor to collect image samples then perform image preprocessing along with feature engineering to extract relevant features.
              
* The solution proposed has very efficiently used each contour present in the pulse sample as a data point henceforth increasing our data points by 20 times with each image. 
* On a test set of 14000 Data points, the model’s efficacy was about 96%, and on a real-life data set of 100 images, it was approximately 87%.
## Technology Stack
* [Visual Studio Code](https://code.visualstudio.com/)
* [Python 3.8.0](https://www.python.org/downloads/release/python-380/)
* [OpenCV](https://opencv.org/)
* [Flutter](https://flutter.dev/)
* [Chaquopy](https://chaquo.com/chaquopy/)
* [EvalML](https://evalml.alteryx.com/en/stable/#)
* 
## Methodology
### Pre-processing
The flow used for pre-processing of data is described below-

![alt text](https://github.com/Subhanshu20101/DaQua-pulse-quality-prediction-model/blob/main/Images/flowchart_pre.png)

### Feature Extraction
We take into account the following physical characterstics- major axis, minor axis, MinbyMaj ratio, Eccentricity, and Grain Area. 

### ML Model Execution
Using AutoML's library EvalML we found the Random Forest Regressor to be the best fit for our feature vector. It comes out to be 99 percent better than baseline model.

### Implenting DaQua App
We implemented the DaQua as a mobile-based application using the Flutter framework, as it works well with both Android and iOS.

![alt text](https://github.com/Subhanshu20101/DaQua-pulse-quality-prediction-model/blob/main/Images/Screenshots%20of%20DaQua%20App.png)

## Some Results
* Importance of each feature plotted using heat map
 
![alt text](https://github.com/Subhanshu20101/DaQua-pulse-quality-prediction-model/blob/main/Images/featureimp.png)

* Confusion matrix

![alt text](https://github.com/Subhanshu20101/DaQua-pulse-quality-prediction-model/blob/main/Images/confusionMatrix.png)

## Contact

Subhanshu Arya - subhanshu20101@iiitnr.edu.in
