# Medical Diagonis webApp
## Our code
we took the dataset from kagel,..., then we filled nan in the columns were no symptom was present. the our dataset looks like this:

Then we printed the unique symptoms from symptom-severity file and applied. Here we used label binarzer, to convert each symptom into a binary matrix, e.g. itching refers to [1,0,0,.....,0] , skin_rashes refers to [0,1,0,0,.....,0] vector. We have 132 symptoms in the dataset.

We have y_vec that has the list of diseases, and x_vec has the list of symptoms. For a corresponding value of x_vec there is a disease. for instance:
ss
