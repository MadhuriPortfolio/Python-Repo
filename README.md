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
<img src="https://github.com/user-attachments/assets/0068d3d4-bb6f-4257-a7c4-b95dfc450499" alt="Description of the Image" width="500" height="300" />
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
<img src="https://github.com/user-attachments/assets/29742f89-820b-4c91-b2ac-02f6bb2c6576" alt="Description of the Image" width="500" height="300" />
</a>
</p>

**3. Write the code to get the information about the DataFrame?**  
df.info()

**4. Write the code to get summary statistics for the DataFrame?**  
summary_stats = df.describe()  
print(summary_stats)  
<p align="left">
<a href="https://your-link.com">
<img src="https://github.com/user-attachments/assets/0801cb44-c876-4fb3-a64a-a890118dd05a" alt="Description of the Image" width="500" height="300" />
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
<img src="https://github.com/user-attachments/assets/4430a9fc-ac4b-4763-9790-7923e2b7a9d2" alt="Description of the Image" width="500" height="300" />
</a>
</p>



