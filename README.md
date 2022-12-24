# Diabetes Machine Learning
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
 


# References
https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset?select=diabetes_binary_health_indicators_BRFSS2015.csv  

