### Marble quality check
  
Data source :  https://www.kaggle.com/wardaddy24/marble-surface-anomaly-detection-2

Data source contains images of marble surfaces. The surfaces are categorised into 4 types : good , crack, joint and dot.  
There are 2249 images for training and validation. 668 images for test purposes.  

#### Model building :  
  
The repo consists of notebooks where in different layers of CNN are built using tensorflow .  
Each model is tested for the performance metrics - individual F1 scores of each class and overall accuracy.  
The model which gives the highest performance metric is selected for cross validation - 3 different slices of train and validation images.  

Its seen that NN with 6 layer convolution and max pooling gives an average accuracy of (0.93 + 0.88 + 0.58)/3 = 0.8. 
  
#### Transfer Learning:  
It is attempted to check if we can use transfer learning from a pretrained model to perform the classification and whether we do get much better accuracy than the built model.  
  
It is seen that using VGG16 model , its trained weights , and by adding a single Dense layer and the the outer layer , we are able to get an accuracy of 0.98.  
  
  
  
    



  

