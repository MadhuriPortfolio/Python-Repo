# Python-Repo  
![python_pandas](https://github.com/user-attachments/assets/7aa8dd18-01a5-4ad2-bf47-2a33f7a8294f) Python is a versatile, high-level programming language known for its simplicity and readability. It is widely used in data analysis, machine learning, web development, and automation. 

In this repository, I showcase various projects that demonstrate my experience with Python, including data manipulation, automation scripts and visualizations.   

**Task 1:** Samples program to print the numbers from 1 to 100, if it is divisble by 3 as 'Fizz' and if a number is divisible by 5 as 'Buzz'. If a number is divisible of by both 3 and 5 then print as "fizzbuzz"   
for i in range(1, 101):
    if i % 3 == 0 and i % 5 == 0:
        print("fizzbuzz", end="  ")  
    elif i % 3 == 0:
        print("fizz", end="  ")  
    elif i % 5 == 0:
        print("buzz", end="  ")  
    else:
        print(i, end="  ")   
<p align="left">
<a href="https://your-link.com">
<img src="https://github.com/user-attachments/assets/0068d3d4-bb6f-4257-a7c4-b95dfc450499" alt="Description of the Image" width="700" height="300" />
</a>
</p>

  
**Task 2:** Down load the file: [student.csv](https://github.com/your-username/your-repository/raw/main/student.csv)  
**1. Write the code to read a CSV file into a Pandas DataFrame
**  df = pd.read_csv('student.csv')  
  df 

**2. Write the code to display the first 5 rows of the DataFrame?**  
df.head()  
<p align="left">
<a href="https://your-link.com">
<img src="https://github.com/user-attachments/assets/29742f89-820b-4c91-b2ac-02f6bb2c6576" alt="Description of the Image" width="700" height="300" />
</a>
</p>

**3. Write the code to get the information about the DataFrame?**  
df.info()

**4. Write the code to get summary statistics for the DataFrame?**  
summary_stats = df.describe()  
print(summary_stats)  
<p align="left">
<a href="https://your-link.com">
<img src="https://github.com/user-attachments/assets/0801cb44-c876-4fb3-a64a-a890118dd05a" alt="Description of the Image" width="700" height="300" />
</a>
</p>


**5. Write the code to select the 'name' and 'mark' columns?**  
selected_columns = df[['name', 'mark']]  
print(selected_columns)
     
**6. Write the code to select all rows where the 'class' is 'Four'?**  
class_four_rows = df[df['class'] == 'Four']  
print(class_four_rows)  
<p align="left">
<a href="https://your-link.com">
<img src="https://github.com/user-attachments/assets/4430a9fc-ac4b-4763-9790-7923e2b7a9d2" alt="Description of the Image" width="700" height="300" />
</a>
</p>

7. Write the code to add a new column 'passed' that indicates whether the student passed (mark >= 60)?
df['passed'] = df['mark'] >= 60  
print(df)
<p align="left">
<a href="https://your-link.com">
<img src="https://github.com/user-attachments/assets/5e6c8774-ba1e-47c9-a4d2-9967bf2e8654" alt="Description of the Image" width="700" height="300" />
</a>
</p>  

8. Write the code to rename the 'mark' column to 'score'?  
df.rename(columns={'mark': 'score'}, inplace=True)  
print(df)  
<p align="left">  
<a href="https://your-link.com">   
<img src="https://github.com/user-attachments/assets/c6b51d99-67f4-47d4-8b0f-c8a62e10351e" alt="Description of the Image" width="700" height="300" />  
</a>
</p> 

9. Write the code to group the DataFrame by the 'class' column and calculate the mean 'mark' for each group?  
group_mean = df.groupby('class')['score’].mean() # Display the result    
print(group_mean)
<p align="left">  
<a href="https://your-link.com">   
<img src="https://github.com/user-attachments/assets/647a653e-1d83-4ba1-bb15-0509cf95bbfa" alt="Description of the Image" width="700" height="300" />  
</a>
</p> 

10. Write the code to calculate the average mark for each gender?   
avg_marks_by_gender = df.groupby('gender')[‘score'].mean()  
print(avg_marks_by_gender)
<p align="left">  
<a href="https://your-link.com">   
<img src="https://github.com/user-attachments/assets/52f96b35-474e-4dcc-8328-bcd1fc718547" alt="Description of the Image" width="700" height="300" />  
</a>
</p> 

11. Write the code to create a pivot table with 'class' as rows, 'gender' as columns, and 'mark' as values?  
pivot_table = df.pivot_table(values='mark', index='class', columns='gender', aggfunc='mean')  
print(pivot_table)
<p align="left">  
<a href="https://your-link.com">   
<img src="https://github.com/user-attachments/assets/bf718de6-88ba-4805-81d9-722f4cbc3132" alt="Description of the Image" width="700" height="300" />  
</a>
</p> 

12. Write the code to create a new column 'grade' where marks >= 85 are 'A', 70-84 are 'B', 60-69 are 'C', and below 60 are 'D'?
<p align="left">  
<a href="https://your-link.com">   
<img src="https://github.com/user-attachments/assets/22479216-cd47-4adf-8fe4-f0e968f48cd0" alt="Description of the Image" width="700" height="300" />  
</a>
</p> 

14. Write the code to save the DataFrame with the new 'grade' column to a new CSV file?  
def assign_grade(mark):  
    if mark >= 85:  
        return 'A'  
    elif mark >= 70:  
        return 'B'  
    elif mark >= 60:   
        return 'C'  
    else:  
        return 'D'  
df['grade'] = df['score'].apply(assign_grade)

# **Task 3: Visualizations in Python**  
<p align="left">  
<a href="https://your-link.com">   
<img src="https://github.com/user-attachments/assets/cc6891e9-9e9c-40f8-85a8-bfe94e51bb57" alt="Description of the Image" width="700" height="300" />  
</a>
</p>  

**Visualize the grade distribution**  
<p align="left">  
<a href="https://your-link.com">   
<img src="https://github.com/user-attachments/assets/be41d18c-89ff-43cb-9c1e-df487c304765" alt="Description of the Image" width="700" height="300" />  
</a>
</p> 

**Student score distribution**
<p align="left">  
<a href="https://your-link.com">   
<img src="https://github.com/user-attachments/assets/e3c79fc5-9e7b-4cf5-90dc-f2aefc3bcc4f" alt="Description of the Image" width="700" height="300" />  
</a>
</p>

**Marks distribution by gender**
<p align="left">  
<a href="https://your-link.com">   
<img src="https://github.com/user-attachments/assets/a7a0fbec-20e4-45a0-adfe-a7f9e59f7f42" alt="Description of the Image" width="700" height="300" />  
</a>
</p>

# Using another data set GDP Down load the file:  
[GDP(nominal)perCapita.csv](https://github.com/your-username/your-repository/raw/main/GDP(nominal)perCapita.csv)   

**Number of countries per Region**  
<p align**="left">  
<a href="https://your-link.com">   
<img src="https://github.com/user-attachments/assets/40641ca5-df8b-4f2f-ab1d-ad2389a016c9" alt="Description of the Image" width="700" height="300" />  
</a>
</p>

**GDP if Europena union countries**
<p align**="left">  
<a href="https://your-link.com">   
<img src="https://github.com/user-attachments/assets/28799aec-4f00-4f5e-adbd-4c01b3fa8ce3" alt="Description of the Image" width="700" height="300" />  
</a>
</p>

**Coutnries in Europe has higher GDP than UK** 
<p align**="left">  
<a href="https://your-link.com">   
<img src="https://github.com/user-attachments/assets/710f837c-eca2-409e-aadf-762268dac96d" alt="Description of the Image" width="700" height="300" />  
</a>
</p>







