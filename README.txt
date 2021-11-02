This would give a brief summary of what I achieved with the dataset.

Improvements on data given to me would be summarized as:
 1. Trained models on the data from 7wells and tested models on the section_2D_1.
 2. Trained models on the data from 7 wells and implemented the SMOTE technique for interpretation on the section_2D_2 data.
 3. Created a new feature or attribute "Sweetness" from Instantaneous Frequency and Amplitude Envelope useful for training models built with the 4 wells data set.
 4. Trained models with data from 4 wells implementing SMOTE technique to handle data inbalance.
 5. Trained models with data from 4 wells implementing GridSearch and K-fold. 
 6. Implemented opposite moving average from exercise 2 on data from 4 wells to increase data for training.

Observations and Findings:
 1. The SMOTE technique was highly successful to handle data inbalance and resulted to great predictions 
     with the SMOTEENN i.e Edited Nearest Neighbours with the best results.
 2. This technique in combination with my defined interval for data and opposite moving average gave the best results on the test data and section_2D_2 data.
 3. The best features for training on the section_2D_2 data were:
    Porosity, Density, Impedance, V_Clay, P_wave and Seismic but the Seismic can't be used in training if the models would be used to predict on the given 3D data.
 4. Prediction on section_2D_1 data was also carried out using models built with data from 7 wells and better results were obtained and this showed clearly 
    the advantage of more data to help build predictive models in this case 7 wells data compared to 4 wells data. 
 5. Predictions on section_2D_1 data with models built from data from 4 wells were improved by implementing SMOTE and using the additional Sweetness attribute generated.
 6. The SMOTE technique was even more successful on data from 4 wells with chosen intervals, moving average implementation k-fold and GridSearch with metrics.
    Mean test score: 1.0 

    Std test score: 0.0 

    Precision/Recall/ F-score on train set : 

    Precision:  1.0
    Recall:  1.0
    F-score:  1.0

    Precision/ Recall/ F-score on validation set : 

    Precision:  1.0
    Recall:  1.0
    F-score:  1.0

    Precision/ Recall/ F-score on test set : 

    Precision:  1.0
    Recall:  1.0
    F-score:  1.0
     
   The above perfect score was gotten from the MLPClassifier where gridSearch and K-fold was implemented and features selected are:
   Porosity, Density, V_Clay, Impedance, and P_wave. This can be checked in the ipynb file called "fourWells_prediction2dNoWells.ipynb"
   The Gaussian Naive Bayes algorithm performed the same but with a thinner prediction on the section_2D_2 data.
   This result can be comparable with results from data from models built from data from 7 wells giving credence to the SMOTE technique employed.

 7.The best algorithm from my observations is the MLPClassifier accross the four ipynb notebooks I created off the notebooks supplied by Elena.

Additional 
  The data for the project would not be found on my git repo because of its size but I am hoping since you supplied the dataset you will still have access to it
  All codes should run smoothly with all data for the project placed in a directory called "data" in the same directory with my ipynb files with datasets as
  provided for the May Geo-python event stored in it namely:
  3D_area.csv, logs_4wells.csv, logs_7wells.csv, section_2D_1.csv, section_2D_2.csv, seismic_4wells.csv, seismic_7wells.csv as this was how the data was initially provided.
  
  Four additional note books named "fourWells_prediction2dNoWells.ipynb", "sevenWells_prediction2dNoWells.ipynb", "fourWells.ipynb", "sevenWells.ipynb"
  are provided for inspection and models stored in directories named "models4wells_2d_1","models7wells_2d_1","mymodels4wells_2d_2","models7wells_2d_2".
  Thanks for the data and codes which I improved on I really learnt a lot.
  I would have provided my solutions earlier but for challenges faced due to power supply and a bad laptop battery.
  Hopefully I get the certificate to add to my portfolio Vita.
  Thanks.

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        