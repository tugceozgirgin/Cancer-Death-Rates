# Cancer-Death-Rates
I conduct a thorough analysis with the goal of applying multiple regression techniques (Ordinary Least Squares, Gradient Descent, KNN Regression) to forecast cancer death rates. To better understand the features of the data, I start by preprocessing and displaying the dataset in order to obtain deeper insights into the correlations between different features and the target variable. After that, I used three distinct regression techniques.

Data Visualization
Understanding linkages and patterns within the dataset requires the use of visualizations. To see how the goal variable (death rate) related to other factors, I used scatter diagrams. While creating the scatter diagrams, I used the Matplotlib library and created all the scatter diagrams for the death rate (target feature) and 33 other features one by one in the for loop. I'm adding a few diagrams below:
![image](https://github.com/tugceozgirgin/Cancer-Death-Rates/assets/93055813/67aac9ab-1777-425f-b5b6-2f54b2b191d9)
![image](https://github.com/tugceozgirgin/Cancer-Death-Rates/assets/93055813/fe4fa312-3a0e-4e0c-b11b-9a5940bf0eb1)
![image](https://github.com/tugceozgirgin/Cancer-Death-Rates/assets/93055813/46b80b2b-6801-4257-ba53-68cb61c5aff9)
![image](https://github.com/tugceozgirgin/Cancer-Death-Rates/assets/93055813/3af07b8b-9c00-4001-a92e-8bfe844adb69)
![image](https://github.com/tugceozgirgin/Cancer-Death-Rates/assets/93055813/4cd3f845-9b92-407a-ad37-d2520607dfdf)

The dataset is divided into training and test sets using the scikit-learn library in each model. The test size was set as 0.2 and the number of random states was set as 271. I used the 1.5 x IQR rule to remove outliers in the final preprocessing stages. In the first stage, I removed the outliers from the model I created by selecting 5 features. Later, when I created the model with the same 5 features without removing them, I realized that removing the outliers did not lead to any advantage. That’s why, for the other models I will mention in this report, I did not remove the outliers using the 1.5 x IQR rule, I only scaled the X values using the MinMax Scaler from the scikit-learn library.

