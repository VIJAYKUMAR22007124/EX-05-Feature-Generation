# EX-05-Feature-Generation


## AIM
To read the given data and perform Feature Generation process and save the data to a file. 

# Explanation
Feature Generation (also known as feature construction, feature extraction or feature engineering) is the process of transforming features into new features that better relate to the target.
 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Clean the Data Set using Data Cleaning Process
### STEP 3
Apply Feature Generation techniques to all the feature of the data set
### STEP 4
Save the data to the file


# CODE
```
import pandas as pd
df = pd.read_csv("Encoding Data.csv")
df

import pandas as pd
df = pd.read_csv("Encoding Data.csv")
from sklearn.preprocessing import LabelEncoder, OrdinalEncoder
data = ["Red","Green","Blue"]
set = OrdinalEncoder(categories = [data])
set.fit_transform(df[["nom_0"]])
df["nom_1"] = set.fit_transform(df[["nom_0"]])
df

data = ["Cold","Warm","Hot"]
st = OrdinalEncoder(categories = [data])
st.fit_transform(df[["ord_2"]])
df["ord_1"] = st.fit_transform(df[["ord_2"]])
df

le = LabelEncoder()
df["sty"]=le.fit_transform(df[["ord_2"]])
df

pd.get_dummies(df,columns=["nom_0"])


import pandas as pd
df = pd.read_csv("Encoding Data.csv")
df
import pandas as pd
df = pd.read_csv("data.csv")
from sklearn.preprocessing import LabelEncoder, OrdinalEncoder
data = ["Cold","Warm","Hot","Very Hot"]
set = OrdinalEncoder(categories = [data])
set.fit_transform(df[["Ord_1"]])
df["nom_1"] = set.fit_transform(df[["Ord_1"]])
df

pd.get_dummies(df,columns=["Ord_1"])

```






# OUPUT

![Screenshot (320)](https://user-images.githubusercontent.com/119657657/233823717-7fe66254-3f64-4b0f-861d-e4b12528207f.png)


![Screenshot (321)](https://user-images.githubusercontent.com/119657657/233823728-f91ce72e-4bd2-4a17-a79a-d7bce7703421.png)


![Screenshot (322)](https://user-images.githubusercontent.com/119657657/233823736-d8902526-8a9b-4bc0-8c09-15bc58b7ac58.png)


![Screenshot (323)](https://user-images.githubusercontent.com/119657657/233823741-3c2ab557-b4f7-40b6-b376-1f555a23d9d0.png)


![Screenshot (324)](https://user-images.githubusercontent.com/119657657/233823751-31489bec-ce81-44ad-95ec-d831dfe3c8c9.png)


![Screenshot (325)](https://user-images.githubusercontent.com/119657657/233823761-5e0071f6-c174-424a-8deb-5844653a1212.png)


![Screenshot (326)](https://user-images.githubusercontent.com/119657657/233823780-9af693e5-7970-4267-945a-6a0499af529f.png)


#RESULT

The given data is read and performed with Feature Generation process and saveed the data to a file. 


