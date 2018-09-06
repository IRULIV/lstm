# Predicting Queue Time with LSTM Classifier
## Bright Uchenna Oparaji, Institute for Risk and Uncertainty, University of Liverpool.

The aim of this project is to build a model and forcast the expected queue time of a HPC resource using recurrent neural network (LSTM).
## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

1) Keras 
2) Numpy
3) Pandas
4) Sklearn
5) os
6) time
7) datetime
### Installing libraries

Install Keras from PyPI (recommended):
```
sudo pip install keras
```
If you are using a virtualenv, you may want to avoid using sudo:
```
pip install keras
```
Alternatively: install Keras from the GitHub source:
First, clone Keras using git:
```
git clone https://github.com/keras-team/keras.git
```
Then, cd to the Keras folder and run the install command:
```
cd keras
sudo python setup.py install
```
Similarly, numpy, pandas, sklearn, os, time and datetime can be installed via pip: 
```
pip install numpy

pip install pandas

pip install sklearn

pip install os

pip install time

pip install datetime
```

## Running the code in IPython console

The main engine of the code is located in lstm_model_final.py. There are three functions (i.e. train_lstm, update_lstm and forcast_with_lstm) inside lstm_model_final.py. train_lstm trains an lstm with the initial training data and displays the reliability of the trained model on training and validation set respectively. Furthermore, a directory named 'model' is created and the trained lstm is stored inside the directory. update_lstm updates the saved model in the directory 'model' when a new training data set is provided. Here, we give a brief demonstration on how to use these functions:
```python
from lstm_model_final import train_lstm, update_lstm, forcast_with_lstm
```
Using the functions:
```python
train_lstm('C:/Users/BRIGHT/Desktop/ZENOTEC_2/Input/TrainingData_Modified.csv')
```
```python
update_lstm('C:/Users/BRIGHT/Desktop/ZENOTEC_2/Input/TrainingData_Update.csv','C:/Users/BRIGHT/Desktop/ZENOTEC_2/Model' )
```
```python
forcast_with_lstm('C:/Users/BRIGHT/Desktop/ZENOTEC_2/Input/TestDataNoOutput.csv','C:/Users/BRIGHT/Desktop/ZENOTEC_2/Model/20180906020843.h5')
```


### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc


