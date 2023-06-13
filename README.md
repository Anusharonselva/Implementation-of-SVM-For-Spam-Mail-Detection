# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Start the program
2. Import the python pandas library as pd
3. Read the contents of the Spam csv file
4. Display the first 5 rows of the dataset using head()
5. Assign x as v1 values and y as v2 values
6. From sklearn library select the feature extraction and import CountVectorizer
7. CountVectorizer will convert the Text to Numerical Data
8. From sklearn library import Support Vector Classifier (ie. SVC)
9. Predict the x_test using SVC
10. Print the accuracy of the SVM Model 11.Stop the program

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: S.ANUSHARON
RegisterNumber:  212222240010

import chardet
file='/content/spam.csv'
with open(file, 'rb') as rawdata:
  result = chardet.detect(rawdata.read(100000))
result  

import pandas as pd
data=pd.read_csv("/content/spam.csv",encoding='windows-1252')

data.head()

data.info()

data.isnull().sum()

x=data["v1"].values

y=data["v2"].values

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

from sklearn.feature_extraction.text import CountVectorizer
cv = CountVectorizer()

x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)

from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred

from sklearn import metrics 
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```

## Output:

Result output:

![Screenshot (313)](https://github.com/Anusharonselva/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119405600/aca6e2c0-87ac-4ace-a1bb-2511d1bc95e3)

data.head():

![Screenshot (313) 1](https://github.com/Anusharonselva/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119405600/a3845035-e759-439c-b567-0c31ae8a2bd5)

data.info():

![Screenshot (314)](https://github.com/Anusharonselva/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119405600/b4e5e687-253d-4076-82c7-4869ce4ca5e8)

data.isnull().sum():

![Screenshot (314) 1](https://github.com/Anusharonselva/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119405600/d8295300-2ea9-4e48-bcbf-feefb15687b2)

Y_Prediction value:

![Screenshot (315)](https://github.com/Anusharonselva/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119405600/cdd1fe33-a3f5-4c64-a5a9-01939544eda5)

Accuracy value:

![Screenshot (315) 1](https://github.com/Anusharonselva/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119405600/68d25a1b-8fed-480c-ae79-4957a82f1b2f)


## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
