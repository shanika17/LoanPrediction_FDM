# LoanPrediction_FDM

Web application : https://loan-prediction-ml-olenzro.herokuapp.com/

Final Report : [FDM_Final_Report_Group22.pdf](https://github.com/shanika17/LoanPrediction_FDM/files/10332003/FDM_Final_Report_Group22.pdf)

Video : 

https://user-images.githubusercontent.com/88156395/210241876-d31cc227-b562-403d-a459-e8fb3ea3357c.mp4

The primary purpose of the project is to measure the risk associated with a client's loan. In this case, a historical data set will be used as a source that contains important characteristics that were collected before lending the loan to customers. So, while finding the solution, the risk of lending the loan will be predicted based on the customers' background which will be identified by key related factors such as annual income, income category, age, house ownership, etc. Accordingly, since the objective is to predict, a predictive model is needed and hence classification technique will be used.

Firstly, the data set will be prepared according to the requirements. After that, the selected dataset will be pre-processed. Following this, using the final tools and technologies, the model will be developed. Then the web application will be designed using specific tools and technologies, and then the model will be integrated with that. Thereafter, the finalized web application will be presented to the end user of the banking sector as the final product, which ends users can use according to their needs. In addition, a video clip will also be given for the convenience of the user, who will describe the process of using the application more simply. Finally, the final report will be provided along with all required details.

The objective of the selected problem and the whole project process is about supplying credit-related services, especially lending loans to customers who are suitable and have a high possibility to pay back.

--Tools and Technoligies

•	Language - Python 

•	IDE - Jupyter, Visual Studio Code 

•	Framework - Flask 

•	Server/Hosting - Heroku 


Following are the steps that followed.

--Analyze the dataset

To get a brief understanding about the dataset, follow these steps.

Step 01: Calculate the size of the dataset with number of features/attributes and check data types of the columns.

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210233644-5a274d25-1b08-4433-b3ba-d175ea94cf83.png">

Step 02: Get an idea about columns and generate column names.

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210233771-2e254b44-5cd9-425e-bb15-1275fc26f0bd.png">

Step 03: Based on the observation of the dataset, plot a diagram to identify the correlation between the features.

<img width="457" alt="image" src="https://user-images.githubusercontent.com/88156395/210233893-47c530e4-f190-4edf-9416-0a455bcf5b05.png">

--Data Preprocessing

Step 01: Identify the null values in the dataset

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210234029-e4ae8b93-5c3c-4b93-8a0f-cc82810461ab.png">

Step 02: Handle numerical missing data with mean and check null values replaced or not

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210234057-e8002fa8-a518-434a-bfb7-e0642c4a35d9.png">

Step 03: Check duplicate values in the dataset

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210234097-72424ffd-46eb-4ca1-872b-07977368cb6d.png">

Step 04: Change the attribute values to a meaningful manner to maintain the consistency between the fields of the training dataset and user inputs

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210234139-7bc2a54d-8bd5-4287-9544-75264f40e9a0.png">

Step 05: Drop columns which are not related and less important like user generated fields

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210234170-0b3a64c5-36fc-42d9-bb9a-b7afd4016c1a.png">

--Data Visualizing

Step 01: Get the plots to get a clear idea about how the features affect to the loan condition.

These are two examples

•	Home ownership status vs loan condition

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210234948-ebf30c27-b88b-42b5-9b3b-0746a7a0df16.png">

•	Income category vs loan condition

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210234982-68f509b6-2b98-4515-8750-08cb723b0444.png">

Step 02: Check numerical data with loan condition

•	Interest rate vs loan condition

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210235183-156af849-4574-4416-96d0-d4828ee3ac58.png">

•	Interest rate box plot

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210235210-53895aa3-e388-4c42-8e50-d790cd32a303.png">

Interest rates have outliers. So, have to remove outliers to reduce the variance of the training data to improve the test accuracy.

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210235261-3065c0a0-7c3d-40fe-867f-9ebaccebeaf2.png">

Step 03: Identify correlation between attributes after the initial preprocessing

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210235554-2b4a43fc-d12c-4f04-8c43-0ccf9ad3acd4.png">

Step 04: Handle the categorical data with OneHotEncoding
  After identifying the categorical attributes have to perform one hot encoding to change them into a numerical attribute. After one hot handling when we check the data type it shows numerical attributes.

--Model Development

* Prediction Model

Step 01: Separating independent and dependent variables

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210236956-f4413cf4-f68c-4d18-82ac-5e5ce1702b51.png">

Step 02: Splitting training and testing data set

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210236993-2a5dab4c-fb5d-4e26-971b-d05f355f640e.png">

* Model Training

01) Logistic Regression

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210240059-6fcfd255-6bbe-402c-96f6-925e2f6d2aa2.png">

02) Random Forest Classifier

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210240140-a83e067e-4ca8-475f-aca3-0f18d9048e47.png">

03) Decision Tree Classifier

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210240218-47b60205-e53c-4fe3-a571-5afc8ff72120.png">

Comparison among the models

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210240303-20de23e2-51c5-4d87-8586-79ee34e6e1cc.png">

Finally choose the Random Forest model because of the accuracy, recall, precision and f1 score is higher than other models. After building the model, to assess the relevance of the features selected, feature importance was performed.

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210240499-0050c170-7c4d-4e66-8836-882065efbdc6.png">

-- UIs of solution

The following screenshots illustrates the user interfaces of the final application deployed to the server. 

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210240611-e641ec79-9d5c-4d63-a427-943d7b919888.png">

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210240633-80f37208-5cc2-4620-ac64-764ef3b2fb0f.png">
<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210240646-427f568a-5f3e-4f7a-9d20-d295b01c7245.png">
<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210240663-5204be88-bcf3-45a6-9f9f-57618e71fd00.png">

Solution Overview with demo

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210240708-38444504-8d7c-45ee-9df4-9260e5fa36f1.png">

After filling the form if the customer suitable for a loan, this will be shown 

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210240751-7dc7f90a-71ec-4066-a6f1-21d9582bf393.png">

After filling the form if the customer not suitable for a loan, this will be shown

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210240793-37543077-70ce-4bfc-b34e-6e4d62ac98db.png">

Accuracy will be displayed shown as below

<img width="468" alt="image" src="https://user-images.githubusercontent.com/88156395/210240832-bb95e1d1-dc09-410a-b2f1-260d36aa2d96.png">
















