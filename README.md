# Data-cleaning
# Data-Cleaning-Activity

## AIM

To read the given data and perform data cleaning and save the cleaned data to a file.

## Explanation

Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

## Algorithm

STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

## Coding & Output

## ACTIVITY 1:

1. Write a Python program to select the 'name' and 'score' columns from the following DataFrame.

Sample DataFrame:

              exam_data = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],

               'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],

              'attempts': [1, 3, 4, 3, 5, 3, 6, 1, 7, 1] } 


![Screenshot (22)](https://github.com/user-attachments/assets/4901c467-0568-42e3-b6fa-5aeb1e1517e1)

![Screenshot (23)](https://github.com/user-attachments/assets/cdb7efd9-a109-4f59-b9eb-0529a88497c8)

2. For the above dataframe, Write a program to select the data who's attempt is greater than 3.

    Code:      df[df['attempts']>3]

![Screenshot (24)](https://github.com/user-attachments/assets/ac68aa19-d84e-4856-a33e-e92742140d7b)

3. Write python code for indexing rows and columns based on the following conditions:

a. Select rows where age is greater than 30:

Code:       df[df['age']>30]

![image](https://github.com/user-attachments/assets/479119ea-e01f-47d9-9c0b-b9527bf46523)

b. Select rows where name contains 'e':

Code:      df[df['name'].str.contains('e')]

![image](https://github.com/user-attachments/assets/2dbbe3ae-36ab-4144-a4d8-73ad934b2689)

c. Select rows where gender is 'M' and salary is greater than 65000:

Code:      df[(df['gender']=='M') & (df['salary']>65000)]

![image](https://github.com/user-attachments/assets/90a24c46-dcbb-4290-93e4-37c125312b2e)

d. Select columns 'name' and 'age' 

Code:     df[['name','age']]

![image](https://github.com/user-attachments/assets/bd24036a-1c07-4d3b-9009-70975f3a284b)

## ACTIVITY 2:

1. Write python code for indexing rows and columns using iloc or loc method based on the following conditions:

Importing dataset

![image](https://github.com/user-attachments/assets/7879051e-7636-4360-b252-a438a9ba18b2)

a.  select the rows where clients with primary education have subscribed to a deposit?

Code:      df.loc[(df['education']=='primary') & (df['deposit']=='yes')]

![image](https://github.com/user-attachments/assets/22333e19-7e93-4fe2-bc3a-665182923c26)

b.  select the rows where clients who have not subscribed to a deposit?

Code:     df.loc[df['deposit']=='no']

![image](https://github.com/user-attachments/assets/fb4ce3e5-f480-4186-a007-48ce6254b8fb)

c. select the rows where clients who have subscribed to a deposit either have a housing or a personal loan?

Code:     df.loc[(df['loan']=='yes') & (df['deposit']=='yes')]

![image](https://github.com/user-attachments/assets/a2d5cb81-e5ce-4824-bdb0-15cd5e027c59)

d. select the rows where clients with secondary education who have not subscribed to a deposit?

Code:     df.loc[(df['education']=='secondary') & (df['deposit']=='no')]

![image](https://github.com/user-attachments/assets/fe9ee2d0-e6be-4261-b0a7-e44ca613d891)

e. select the rows where  clients who have subscribed to a term deposit as an outcome of the successful marketing campaign?

Code:    df.loc[(df['poutcome']=='success') & (df['deposit']=='yes')]

![image](https://github.com/user-attachments/assets/7b7a3d60-c675-4fd6-9bd6-8b054ab9a03a)

f. select the rows where unemployed clients who have not subscribed to deposit?

Code:     df.loc[(df['job']=='unemployed') & (df['deposit']=='no')]

![image](https://github.com/user-attachments/assets/c8e11d6a-8d9a-4e68-a9ea-e94538e7e457)


g.select coloumns ‘education’ and ‘balance’ where age is less than or equal to 30.

Code:     df.loc[df['age']>30,['education','balance']]

![image](https://github.com/user-attachments/assets/41eddfa8-c81e-4f66-906f-ee7b5364b615)

## Result
Thus the data cleaning process has been executed successfully.
