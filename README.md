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
![SVM For Spam Mail Detection](sam.png)

![Screenshot (97)](https://github.com/Anusharonselva/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119405600/327d8488-f0cd-487e-9823-5134452a5ce6)

![Screenshot (98)](https://github.com/Anusharonselva/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119405600/7ae4ea3d-88b3-4087-8237-0cdda66d1f5a)

![Screenshot (98) 1](https://github.com/Anusharonselva/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119405600/1a9a906e-33fe-432a-af40-567fac921b03)

![Screenshot (99)](https://github.com/Anusharonselva/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119405600/4d91a9e9-105c-416c-a8d3-73e465c82718)

![99 1](https://github.com/Anusharonselva/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119405600/7a9466e9-bdb9-4e23-bcb2-0df08b741bb8)


## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
