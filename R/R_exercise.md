### BEGINNER EXERCISES
1.1 Hello, R!
Write a simple R script that prints the message "Hello, R!" to
the console.
1.2 Basic Arithmetic Operations
Create a script that performs the following arithmetic
operations:
1.2.1 Addition of 5 and 7
1.2.2 Subtraction of 10 from 15
1.2.3 Multiplication of 3 by 4
1.2.4 Division of 20 by 5
1.3 Variable Declaration
Declare a variable called my_number and assign it the value
42. Print the value to the console.
1.4 Vector Creation
Create a numeric vector named my_vector containing the
numbers 1 to 5. Print the vector.
1.5 Vector Operations
Perform the following operations on the vector my_vector:
1.5.1 Multiply each element by 2
1.5.2 Add 3 to each element
Print the updated vector.
1.6 Logical Operations
Declare two variables, x and y, with values 5 and 10,
respectively. Check if x is less than y and print the result.
1.7 Data Types
Create variables of different data types: numeric, character,
logical, and print them.
1.8 Basic Data Frame
Create a data frame named my_dataframe with two
columns: "Name" and "Age," and enter information for three
people.
1.9 Indexing in Vectors
Given the vector letters_vector <- c("A", "B", "C", "D", "E"),
print the third element.
1.10 Subsetting Data Frames
From my_dataframe, select and print the row where the age
is greater than 25.
1.11 Conditional Statements
Write a script that checks if a variable num is even or odd
and prints an appropriate message.
1.12 For Loop
Use a for loop to print the numbers from 1 to 5.
1.13 While Loop
Implement a while loop that prints the squares of numbers
from 1 to 4.
1.14 Functions
Create a function called square that takes a number as an
argument and returns its square.
1.15 Packages
Install and load the "dplyr" package. Create a simple data
frame and use the filter function to subset it.
1.16 Reading Data
Read a CSV file named "data.csv" into a data frame called
my_data.
1.17 Plotting
Create a scatter plot with my_dataframe where "Age" is on
the x-axis and "Name" is on the y-axis.
1.18 Random Numbers
Generate a vector of 5 random numbers between 1 and 10.
1.19 Strings and Manipulation
Declare a character variable my_string with the value
"Hello, World!" and print its length.
1.20 Basic Error Handling
Write a script that attempts to divide a number by zero and
handle the resulting error with an informative message.
### INTERMEDIATE EXERCISES
2.1 Functions with Default Arguments
Create a function named power that takes two
arguments, base and exponent, with the default
exponent set to 2. The function should return the result
of raising the base to the exponent.
2.2 Data Frame Manipulation
Given a data frame named grades with columns
"Name," "Math," and "English," add a new column called
"Total" representing the sum of Math and English scores.
2.3 Conditional Data Frame Manipulation
From the grades data frame, create a new data frame
containing only the rows where the total score is greater
than 150.
2.4 List Manipulation
Create a list named my_list with the following elements:
a numeric vector, a character vector, and a logical
vector. Print each element separately.
2.5 List Operations
Add a new element to my_list containing a factor vector.
Print the updated list.
2.6 Apply Functions
Using the apply function, calculate the mean of each
column in the grades data frame.
2.7 Matrix Operations
Create a 3x3 matrix with random numeric values.
Calculate the sum of each row and each column.
2.8 Subsetting with Conditions
Extract rows from the grades data frame where both
Math and English scores are above the mean of their
respective columns.
2.9 File Writing
Write the grades data frame to a CSV file named
"student_grades.csv."
2.10 Error Handling in Functions
Modify the power function from question 2.1 to include
error handling. If the base is negative, print an error
message.
2.11 Loading External Data
Load the "iris" dataset from the datasets package.
Display the first 5 rows.
2.12 Data Frame Joining
Create two data frames, students and courses, with
columns "StudentID" and "CourseID" respectively.
Perform an inner join based on these columns.
2.13 Reshaping Data
Convert the grades data frame from wide to long format
using the melt function from the reshape2 package.
2.14 Time Series Creation
Create a time series object with daily values from
January 1, 2023, to January 10, 2023.
2.15 Plotting with ggplot2
Use ggplot2 to create a scatter plot of the "iris" dataset
with Sepal.Length on the x-axis and Sepal.Width on the
y-axis, color-coded by species.
2.16 String Manipulation with Regular Expressions
Given a character vector containing email addresses,
extract only the domain names (e.g., "gmail.com").
2.17 Creating a Shiny App
Install the shiny package and create a simple Shiny app
with a numeric input and a plot that displays the square
of the input.
2.18 Building a Function Pipeline
Create a function pipeline using the magrittr (%>%)
operator to take the mean, square, and then sum a
numeric vector.
2.19 Hierarchical Clustering
Apply hierarchical clustering to the "iris" dataset and
plot the resulting dendrogram.
2.20 Parallel Processing
Use the parallel package to parallelize the calculation of
the mean for each column in the grades data frame.

### ADVANCED EXERCISES 
3.1 Advanced Function
Create a function named fibonacci that generates
the Fibonacci sequence up to a specified term n.
3.2 Advanced Data Frame Manipulation
Given a data frame named sales with columns
"Date," "Product," and "Revenue," calculate the
rolling 7-day average revenue for each product.
3.3 Advanced List Manipulation
Create a nested list representing a 3x3x3 array of
numeric values. Use indexing to access and print
a specific element within the array.
3.4 Advanced Apply Functions
Utilize the purrr package to apply a custom
function that takes a numeric vector and returns
a list with the mean, standard deviation, and
skewness.
3.5 Advanced Matrix Operations
Implement matrix multiplication without using the
%*% operator. Define a function that takes two
matrices as input and returns their product.
