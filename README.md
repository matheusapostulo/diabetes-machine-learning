# DIABETES MACHINE LEARNING
We will build two classification models, one with Bayes and the other with Forest Random. In the end, we'll do a comparison between the two to see which had better accuracy in predicting diabetes.

# DATA PRE PROCESSING
## DATA EXPLORATION 
- Duplicate rows may be a problem with model accuracy. Let's consider deleting the rows if necessary.  
![image](https://user-images.githubusercontent.com/73514316/209403884-51e8ed62-c7e3-4b18-a77f-9055dbea86a8.png)  
  
- The others issues seem right!
  
  
## DATA VISUALIZATION  
### Possible outliers
However, they don't seem to be outliers that will cause problems for the models.
![image](https://user-images.githubusercontent.com/73514316/209413129-2bf92635-95b1-4ec9-8fb6-cff449a98544.png)

**Graphics**  
![image](https://user-images.githubusercontent.com/73514316/209413198-665b77a4-cc2f-40a8-91ce-4d965656a4d8.png)
![image](https://user-images.githubusercontent.com/73514316/209413205-84726220-522a-4ba2-bc22-0035e43a8da1.png)
![image](https://user-images.githubusercontent.com/73514316/209413262-21a00ada-c869-4843-a6af-eee764b607dd.png)
![image](https://user-images.githubusercontent.com/73514316/209413277-ff2cb9a7-25bb-45ff-b237-3eacc458b8a1.png)

### Missing values analysis
No missing values!!  
![image](https://user-images.githubusercontent.com/73514316/209403138-8e9f4bcc-90b1-4f4f-9444-27351ab368d2.png)  


## SCALING AND TREATMENT OF CATEGORICAL ATTRIBUTES  
It wasn't necessary because the dataframe was already clean.

## SPLIT OF BASES INTO TRAINING AND TESTING
A commonly used ratio is 80:20, which means 80% of the data is for training and 20% for testing.  
![image](https://user-images.githubusercontent.com/73514316/209414553-dec1257e-900b-46ff-b14f-0ffe50c80248.png)
  
So this is how our bases were divided:  
![image](https://user-images.githubusercontent.com/73514316/209414584-b9974b7f-fedf-4210-9879-1d43c0d868ab.png)
 
# COMPARING RESULTS BETWEEN BAYES AND FOREST RANDOM (3 DATASETS)
## DIABETES IMBALANCE
### BAYES - 75.95%  
![image](https://user-images.githubusercontent.com/73514316/209579885-65ded819-e936-482f-bdf8-b7376efab1f5.png)

### FOREST RANDOM - 84.13%  
![image](https://user-images.githubusercontent.com/73514316/209580042-0b50b8d9-8868-49b9-845a-2092e0bd5184.png)

## DIABETES IMBALANCE (WITHOUT DUPLICATE ROWS)  
We didn't get better resuls by deleting duplicate rows!
### BAYES - 73.99%
![image](https://user-images.githubusercontent.com/73514316/209580228-ed0d42f4-12b0-48d3-a0e2-85ce0682616f.png)

### FOREST RANDOM - 82.11%    
![image](https://user-images.githubusercontent.com/73514316/209580238-9099c9c9-cc79-4f96-bbeb-46bc5a8f99cc.png)

## DIABETES BINARY IMBALANCE  
### BAYES - 77.66%
![image](https://user-images.githubusercontent.com/73514316/209580308-374cc669-e442-4f0e-96bc-ea06a5e307d1.png)

### FOREST RANDOM - 85.78%
![image](https://user-images.githubusercontent.com/73514316/209580321-a9793e54-19fb-40ac-9dda-785364165d9e.png)

## DIABETES BINARY BALANCE  
### BAYES - 72.25%
![image](https://user-images.githubusercontent.com/73514316/209580370-a8a04725-d369-409a-af66-435c964eb98f.png)

### FOREST RANDOM - 73.64%
![image](https://user-images.githubusercontent.com/73514316/209580382-cb430593-22ee-4de2-bf5d-70a7c6ecda47.png)

# CONCLUSIONS 
Therefore, we achieved the best result (85.78% accuracy) using the dataset "DIABETES BINARY IMBALANCE" (Binary -> 0 = no diabetes, 1= prediabetes or diabetes) with the **Forest Random algorithm**.

# References
https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset?select=diabetes_binary_health_indicators_BRFSS2015.csv  

