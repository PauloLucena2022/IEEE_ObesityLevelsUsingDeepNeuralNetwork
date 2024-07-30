# Code for predict obesity levels using deep neural networks and data pre-processing

Resources and extra documentation for the manuscript "Predictive Performance of Machine Learning Algorithms Regarding Obesity Levels Based on Physical Activity and Nutritional Habits: A Comprehensive Analysis" published in IEEE Latin America Transactions. 
The code is organized for type of process: 

* Pre-processing: Python;
* Deep Learning predictions: C;
* Other algorithms to predict: Weka.
------------------------------------------------
## Dataset and subsets

The database files are in the folder "Dataset - Obesity Levels Based on Eating Habits and Physical Condition in Individuals". In this folder, you will find the original database - ObesityDataSet_raw_and_data_sinthetic.csv.csv - and the subdivisions used for K-fold cross validation in the "K-fold cross validation" folder. In this folder, the divisions are separated as k = 2, k = 3, k = 4, and k = 5, and within them, the subdivisions for each specific case are labeled as D1, D2, D3, D4, etc. - all in txt format for copying and pasting into the code.

## Codes

### Pré processing

The code for preprocessing is in the folder "PYTHON - Pre-processing code," where you can find the script used to prepare the database for use in the neural network. In this Python notebook, you just need to use the previously described CSV database.

### Predict

The prediction codes are in two folders: "C - Algorithms for deep learning prediction," which contains the deep neural networks using C, and "WEKA - Algorithms for other predictions," which contains the algorithms for J48, Naive-Bayes, Multiclass Classification, and KNN.
In the C codes, there are folders for the three networks used - 3C, 3C recurrent, and 4C. Inside each folder, there are the k-fold cross validation divisions - K = 2, K = 3, K = 4, and K = 5. Within each of these folders, you will find the architectures used in the article. Inside each architecture folder, the codes are separated by k-fold test. For example, if K = 2, there will be "D1 training - D2 testing," meaning D1 was used to train the network and D2 was used to test the network, and so on.

Note: Although the databases are in a separate folder, all C codes already have their respective data set subdivisions placed in the training and testing sections, so they can be compiled directly.


  
