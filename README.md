# Medical Diagonis webApp
## Our code
we took the dataset from Kaggle, Disease Symptom Dataset, then we filled nan in the columns were no symptom was present, then our dataset looks like this:
![](https://github.com/Ananyaiitbhilai/Assignment1c/blob/main/images/Screenshot%202022-02-21%20at%2012.39.05%20AM.png)<br>

We printed the unique symptoms from symptom-severity csv file and applied label binarizer to each symptom. Here we used label binarzer, to convert each symptom into a binary matrix, e.g. itching refers to [1,0,0,.....,0] , skin_rashes refers to [0,1,0,0,.....,0] vector. We have 132 symptoms in the dataset. This implies we have length of array as 132.

We have y_vec that has the list of diseases, and x_vec has the list of symptoms. For a corresponding value of x_vec there is a y_vec i.e. a disease. for instance:
![](https://github.com/Ananyaiitbhilai/Assignment1c/blob/main/images/Screenshot%202022-02-21%20at%201.09.48%20AM.png)<br>

It is being interpreted as:
![](https://github.com/Ananyaiitbhilai/Assignment1c/blob/main/images/Screenshot%202022-02-21%20at%201.14.05%20AM.png)<br>


We splitted the data into testing and training(85%).
We used inbuit decision tree function and saved the trained model in a pickel file. We got an accuracy of 100%, and the following confusion matrix.
![](https://github.com/Ananyaiitbhilai/Assignment1c/blob/main/images/Screenshot%202022-02-21%20at%201.19.12%20AM.png)<br>
![](https://github.com/Ananyaiitbhilai/Assignment1c/blob/main/images/Screenshot%202022-02-21%20at%201.19.27%20AM.png)<br>


Here even if the order of symptoms are changed i.e. order is shufffled, same disease is predicted. for e.g.
![](https://github.com/Ananyaiitbhilai/Assignment1c/blob/main/images/Screenshot%202022-02-21%20at%201.21.18%20AM.png)<br>
![](https://github.com/Ananyaiitbhilai/Assignment1c/blob/main/images/Screenshot%202022-02-21%20at%201.24.51%20AM.png)<br>


