# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the required libraries.
2. Upload the csv file and read the dataset.
3. Check for any null values using the isnull() function.
4. From sklearn.tree inport DecisionTreeRegressor.
5. Import metrics and calculate the Mean squared error.
6. Apply metrics to the dataset, and predict the output.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: MEENA .S
RegisterNumber:  212221240028
import pandas as pd
data = pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
data["Position"] = le.fit_transform(data["Position"])
data.head()
x = data[["Position","Level"]]
y = data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt = DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
from sklearn import metrics
mse = metrics.mean_squared_error(y_test,y_pred)
mse
r2 = metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
*/
```
## Output:
## Read Data:
![image](https://user-images.githubusercontent.com/94677128/173624720-a30db56a-162d-4acd-a09b-e33dc9ef46b3.png)
## Data Info:
![image](https://user-images.githubusercontent.com/94677128/173624855-de1f9a33-5a0d-4e19-92e2-c0bde4468c24.png)
## Null values:
![image](https://user-images.githubusercontent.com/94677128/173624942-98481cbc-0ce0-499e-bffe-1242abe6da10.png)
## After applying LabelEncoder:
![image](https://user-images.githubusercontent.com/94677128/173625045-94e99520-3a05-433c-a574-2ea75d156a25.png)
## Mean Square Error(MSE):
![image](https://user-images.githubusercontent.com/94677128/173625144-5666723a-2c03-4ec3-a4dc-94ec88b10fe5.png)
## R square(r^2):
![image](https://user-images.githubusercontent.com/94677128/173625258-0aff0c04-2b45-4802-afe2-24fcc4cecbaf.png)
## Data Prediction:
![image](https://user-images.githubusercontent.com/94677128/173625367-f4276ebf-1268-44f2-b454-bdd00f9dc61c.png)



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
