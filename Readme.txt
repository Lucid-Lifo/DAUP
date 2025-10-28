1. Swap two variables (temp variable).
2. Count vowels in a string.
3. Reverse a string (no built-in functions).
4. Concatenate two strings.
5. Check if substring exists.
6. Find min/max in a list.
7. Remove duplicates from a list.
8. Calculate tuple sum and average.
9. Find the second largest number in a list.
10. Count element frequency in a list.
11. Find set union and intersection.
12. Print dictionary keys and values.
13. Count character frequency in a string (using a dictionary).
14. Print prime numbers (1-50).
15. Generate a multiplication table from user input.
16. Print Fibonacci series up to n terms.
17. Create a Calculator class (add, subtract, multiply, divide).
18. Demonstrate multilevel inheritance (e.g., Vehicle > Car > ElectricCar).
19. Implement polymorphism (e.g., Shape > Rectangle/Circle area).
20. Count words, lines, and characters in a file.
21. Demonstrate file I/O methods (read, readline, write, etc.).
22. Print current date, time, and day.
23. Calculate age from date of birth.
24. Handle DivisionByZero exception.
25. Create and raise a custom exception.
26. Use a try-except-else-finally block.
27. Connect to MySQL.
28. Connect to SQLite3.
29. Implement database CRUD operations.
30. Create a CGI login form.
31. Create a CGI registration form.
32. Perform MySQL CRUD operations using CGI.
33. NumPy: Create an array of ones.
34. NumPy: Remove rows with non-numeric values.
35. NumPy: Remove single-dimensional entries (squeeze).
36. NumPy: Check if values exist in an array.
37. NumPy: Sort an array (by axis and flat).
38. NumPy: Create and sort a structured array (e.g., by class, then height).
39. NumPy: Sort a complex array (by real, then imaginary part).
40. NumPy: Sort an array by the nth column.
41. NumPy: Calculate the sum of diagonal elements (trace).
42. NumPy: Matrix multiplication.
43. NumPy: Multiply complex matrices.
44. NumPy: Compute covariance matrix.
45. NumPy: Convert covariance to correlation matrix.
46. NumPy: Compute a histogram.
47. NumPy: Compute cross-correlation.
48. NumPy: Calculate mean, std, and variance along an axis.
49. Data Viz: Line plot of stock prices.
50. Data Viz: Bar plot of trading volume.
51. Data Viz: Stacked histogram of stock prices.
52. Data Viz: Scatter plot of volume vs. price.
53. Data Preprocessing: Handle missing values.
54. Data Preprocessing: Encode categorical data.
55. Data Preprocessing: Scale features.
56. Data Preprocessing: Normalize data.
57. Machine Learning: Compare 3 classification models to predict user purchases.
58. Machine Learning: Comparative study of classification algorithms.
59. Titanic 

Program 1:Write a Python program to swap two variables using a temporary variable.
a = 10
    b = 20
    print(f"Before swapping: a = {a}, b = {b}")
    temp = a
    a = b
    b = temp
    print(f"After swapping: a = {a}, b = {b}")

Program 2:Write a program that takes a user input string and returns the number of vowels
text = input("Enter a string: ")
    vowels = "aeiouAEIOU"
    count = 0
    for char in text:
        if char in vowels:
            count += 1
    print(f"Number of vowels: {count}")

Program 3:Write a program to reverse a string without using built -in functions.
text = input("Enter a string: ")
reversed_text = text[:: -1]
print(f"Reversed string: {reversed_text}")

Program 4:Concatenate two strings using variables and print the result.
str1 = "Hello"
str2 = "World"
result = str1 + " " + str2
print(f"Concatenated string: {result}")

Program 5:Write a program that checks whether a substring exists in a given string.
main_string = input("Enter main string: ")
substring = input("Enter substring to search: ")
if substring in main_string:
  print(f"'{substring}' exists in '{main_string}'")
else:
  print(f"'{substring}' does not exist in '{main_string}'")

Program 6:Write a program to find the maximum and minimum elements in a list.
numbers = [5, 3, 8, 1, 9, 2, 7]
maximum = numbers[0]
minimum = numbers[0]
for num in numbers:
 if num > maximum:
        maximum = num
    if num < minimum:
        minimum = num
print(f"List: {numbers}")
print(f"Maximum: {maximum}, Minimum: {minimum}")

Program 7:Write a program to remove duplicates from a list.
original_list = [1, 2, 2, 3, 4, 4, 5, 6, 6, 7]
    unique_list = []

    for item in original_list:
        if item not in unique_list:
            unique_list.append(item)

    print(f"Original list: {original_list}")
    print(f"List without duplicates: {unique_list}")

Program 8:Create a tuple of 5 numbers. Print the sum and average of the numbers.
numbers = (10, 20, 30, 40, 50)
    total_sum = sum(numbers)
    average = total_sum / len(numbers)

    print(f"Tuple: {numbers}")
    print(f"Sum: {total_sum}")
    print(f"Average: {average}")

Program 9:Write a program to find the second largest number in a list.
numbers = [5, 3, 8, 1, 9, 2, 7]
    numbers_sorted = sorted((numbers),reverse=True)

    if len(numbers_sorted) >= 2:
        second_largest = numbers_sorted[1]
        print(f"List: {numbers}")
        print(f"Second largest: {second_largest}")
    else:
        print("List doesn't have enough unique elements")

Program 10:Write a Python function to count how many times an element appears in a list.
def count_occurrences(lst, element):
    count = 0
    for item in lst:
        if item == element:
            count += 1
    return count
numbers = [1, 2, 3, 4, 2, 2, 5, 1]
print(numbers)
print(f"the number 2 appear",count_occurrences(numbers, 2),"times")
print(f"the number 1 appear",count_occurrences(numbers, 1),"times")
print(f"the number 6 appear",count_occurrences(numbers, 6),"times")

Program 11:Write a program to find the union and intersection of two sets.
set1 = {1, 2, 3, 4, 5}
    set2 = {4, 5, 6, 7, 8}
    union = set1 | set2
    intersection = set1 & set2
    print(f"Set 1: {set1}")
    print(f"Set 2: {set2}")
    print(f"Union: {union}")
    print(f"Intersection: {intersection}")

Program 12:Create a dictionary with 5 key -value pairs and print all keys and values.
student_grades = {
        "Alice": 85,
        "Bob": 90,
        "Charlie": 78,
        "Diana": 92,
        "Eve": 88
    }
    print("Keys:", list(student_grades.keys()))
    print("Values:", list(student_grades.values()))

Program 13:Write a program to count the frequency of characters in a string using a
text = input("Enter a string: ")
    freq_dict = {}
    for char in text:
        if char in freq_dict:
            freq_dict[char] += 1
        else:
            freq_dict[char] = 1
    print("Character frequencies:")
    for char, freq in freq_dict.items():
        print(f"'{char}': {freq}")

Program 14:Write a program to print all prime numbers between 1 and 50.
for n in range(2,51):
  flag=False
  for i in range(2,int(n**0.5)+1):
    if(n%i==0):
      flag=True
      break
  if flag==False:
    print(n)

Program 15:Write a program to take user input and generate the multiplication table of the
num = int(input("Enter a number: "))
    print(f"Multiplication table of {num}:")
    for i in range(1, 11):
        result = num * i
        print(f"{num} × {i} = {result}")

Program 16:Write a program to print Fibonacci series up to n terms.
n = int(input("Enter the number of terms: "))
a, b = 0, 1
if n <= 0:
    print("Please enter a positive integer.")
elif n == 1:
    print(a)
else:
    print(a, b, end=' ')
    for i in range(2, n):
        c = a + b
        print(c, end=' ')
        a, b = b, c

Program 17:Create a Calculator class with methods add, subtract, multiply, divide.
class Calculator:
    def add(self, x, y):
        return x + y
    def subtract(self, x, y):
        return x - y
    def multiply(self, x, y):
        return x * y
    def divide(self, x, y):
        if y == 0:
            return "Error: Division by zero"
        return x / y
calc = Calculator()
print(f"3 + 5 = {calc.add(3, 5)}")
print(f"10 - 4 = {calc.subtract(10, 4)}")
print(f"6 * 7 = {calc.multiply(6, 7)}")
print(f"20 / 5 = {calc.divide(20, 5)}")
print(f"10 / 0 = {calc.divide(10, 0)}")

Program 18:Implement a Vehicle → Car → ElectricCar hierarchy and demonstrate multilevel
class Vehicle:
    def __init__(self, brand):
        self.brand = brand
 def display_info(self):
        print(f"Brand: {self.brand}")
class Car(Vehicle):
    def __init__(self, brand, model):
        super().__init__(brand)
        self.model = model
    def display_info(self):
        super().display_info()
        print(f"Model: {self.model}")
class ElectricCar(Car):
    def __init__(self, brand, model, battery_range):
        super().__init__(brand, model)
        self.battery_range = battery_range
    def display_info(self):
        super().display_info()

        print(f"Battery Range: {self.battery_range} miles")
# Demonstrate multilevel inheritance
my_electric_car = ElectricCar("Tesla", "Model 3", 350)
my_electric_car.display_info()

Program 19:Create a Shape base class with a method area(). Derive Rectangle and Circle
import math
class Shape:
    def area(self):
        """Calculates the area of the shape."""
        return 0
class Rectangle(Shape):
    def __init__(self, width, height):
        self.width = width
        self.height = height
    def area(self):
        """Calculates the area of the rectangle."""
        return self.width * self.height
class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius
    def area(self):
        """Calculates the area of the circle."""
        return math.pi * self.radius**2


rectangle = Rectangle(5, 10)
circle = Circle(7)
print(f"Area of Rectangle: {rectangle.area()}")
print(f"Area of Circle: {circle.area()}")

Program 20:Write a program to read a text file and count words, lines, and characters.
with open("sample.txt", "w") as f:
    f.write("This is the first line. \n")
    f.write("This is the second line with more words. \n")
    f.write("Third line.")
def count_file_contents(filename):
    try:
        with open(filename, 'r') as f:
            lines = f.readlines()
            line_count = len(lines)
            char_count = sum(len(line) for line in lines)
            word_count = sum(len(line.split()) for line in lines)

        return line_count, word_count, char_count

    except FileNotFoundError:
        return "Error: File not found."

filename = "sample.txt"
line_count, word_count, char_count = count_file_contents(filename)

if isinstance(line_count, int):
    print(f"File: {filename}")
    print(f"Number of lines: {line_count}")
    print(f"Number of words: {word_count}")
    print(f"Number of characters: {char_count}")
else:
    print(line_count)

Program 21:Demonstrate use of read(), readline(), readlines(), write(), and writelines().
with open("write_demo.txt", "w") as f:
    f.write("This is the first line written with write(). \n")
    f.writelines(["This is the second line written with writelines(). \n", "This is the third line also
with writelines(). \n"])
with open("write_demo.txt", "r") as f:
    content = f.read()
    print("Content using read():")
    print(content)
 Demonstrate readline()
with open("write_demo.txt", "r") as f:
    print(" \nContent using readline():")
    print(f.readline(), end='')
    print(f.readline(), end='')

# Demonstrate readlines()
with open("write_demo.txt", "r") as f:
    print(" \nContent using readlines():")
    lines = f.readlines()
    print(lines)

Program 22:Print current date, time, and day of the week.
from datetime import datetime

now = datetime.now()

print(f"Current Date and Time: {now}")
print(f"Current Date: {now.date()}")
print(f"Current Time: {now.time()}")
print(f"Day of the week: {now.strftime('%A')}")

Program 23:Write a program to calculate age from a given date of birth.
from datetime import date
def calculate_age(birth_date):
    today = date.today()
    age = today.year - birth_date.year - ((today.month, today.day) < (birth_date.month,
birth_date.day))
    return age
dob = date(1990, 5, 15)
age = calculate_age(dob)
print(f"The age for date of birth {dob} is: {age}")

Program 24:Write a program to handle division by zero exception.
def safe_division(numerator, denominator):
    try:
        result = numerator / denominator
        return result
    except ZeroDivisionError:
        return "Error: Division by zero is not allowed."

print(f"10 / 2 = {safe_division(10, 2)}")
print(f"5 / 0 = {safe_division(5, 0)}")

Program 25:Create a custom exception class NegativeValueError and raise it when negative
class NegativeValueError(Exception):
    """Custom exception raised for negative input values."""
    pass
def process_positive_number(number):
    if number < 0:
        raise NegativeValueError("Input must be a non -negative number.")
    return f"Processing positive number: {number}"
try:
    print(process_positive_number(10))
    print(process_positive_number( -5))
except NegativeValueError as e:
    print(f"Caught exception: {e}")

Program 26:Demonstrate use of try -except -else-finally
def divide_numbers(a, b):
    try:
        result = a / b
    except ZeroDivisionError:
        # This block is executed if a ZeroDivisionError occurs in the try block
        print("Error: Division by zero is not allowed.")
    except TypeError:
        # This block is executed if a TypeError occurs
        print("Error: Invalid input types. Please use numbers.")
    else:
        # This block is executed if the try block completes without raising an exception
        print(f"Division successful. Result: {result}")
    finally:
        # This block is always executed, regardless of whether an exception occurred or not
        print("Execution of divide_numbers function is complete.")


divide_numbers(10, 2)
print(" -" * 20)

divide_numbers(5, 0)
print(" -" * 20)
divide_numbers(10, "a")

Program 27:Implementation of MySQL connection using Python
import mysql.connector
from mysql.connector import Error

def connect_to_mysql():
    """ Establishes and closes a connection to a MySQL database. """
    connection = None
    try:
        connection = mysql.connector.connect(
            host="localhost",
            user="root",
            password="",
            database="testdb"
        )

        if connection.is_connected():
            # --- This is the corrected line ---
            # 'server_version' returns a tuple like (10, 4, 32)
            version_tuple = connection.server_version
            # We format it into a nice string
            db_info = ".".join(map(str, version_tuple))
            print(f"Successfully connected to MySQL Server version {db_info}")

    except Error as e:
        print(f"Error while connecting to MySQL: {e}")

    finally:
        if connection and connection.is_connected():
            connection.close()
            print("MySQL connection is now closed.")

if __name__ == '__main__':
    connect_to_mysql()

Program 28:Implementation of SqLite3 connection using Python
import sqlite3
from sqlite3 import Error

def connect_to_sqlite():
    connection = None
    try:
        connection = sqlite3.connect("mydatabase.db")
        print(f"Successfully  connected to SQLite database (version {sqlite3.sqlite_version})")

    except Error as e:
        print(f"Error while connecting to SQLite: {e}")

    finally:
        if connection:
            connection.close()
            print("SQLite connection is now closed.")

if __name__ == '__main__':
    connect_to_sqlite()

Program 29:Write a program to implement CRUD operations using Python

import sqlite3
conn = sqlite3.connect("crud_example.db")
cursor = conn.cursor()
cursor.execute("""
CREATE TABLE IF NOT EXISTS students (
 id INTEGER PRIMARY KEY AUTOINCREMENT,
 name TEXT,
 age INTEGER,
 course TEXT
)
""")
def create(name, age, course):
 cursor.execute("INSERT INTO students (name, age, course) VALUES (?, ?, ?)",
(name, age, course))
 conn.commit()
def read():
 cursor.execute("SELECT * FROM students")
 for row in cursor.fetchall():
 print(row)
def update(student_id, name, age, course):
 cursor.execute("UPDATE students SET name=?, age=?, course=? WHERE id=?",(name, age, course, student_id))
 conn.commit()
def delete(student_id):
 cursor.execute("DELETE FROM students WHERE id=?", (student_id,))
 conn.commit()
create("Alice", 21, "Computer Science")
create("Bob", 22, "Mathematics")
print("All Records:")
read()
update(1, "Alice Johnson", 22, "AI & ML")
print("\nAfter Update:")
read()
delete(2)
print("\nAfter Delete:")
read()
conn.close()


or

import sqlite3
from sqlite3 import Error
def getconn():
    conn=sqlite3.connect('student.db')
    conn.row_factory=sqlite3.Row
    return conn
def createtable():
    conn=getconn()
    try:
        conn.execute('''CREATE TABLE IF NOT EXISTS studinfo (id integer PRIMARY KEY AUTOINCREMENT,name TEXT NOT NULL,mark INTEGER)''')
        conn.commit()
        print("table created")
        conn.close()
    except Error as e:
        print(e)
def adddata():
    name=input("Enter name")
    mark=int(input("mark:"))
    conn=getconn()
    try:
        conn.execute('INSERT INTO studinfo (name,mark) VALUES(?,?)',(name,mark))
        conn.commit()
        print("Data added")
        conn.close()
    except Error as e:
        print(e)
def viewdata():
    conn=getconn()
    try:
        user=conn.execute('Select * from studinfo').fetchall()
        for i in user:
            print(f"ID={i['id']},Name={i['name']},Mark={i['mark']}")
        conn.close()
    except Error as e:
        print(e)
def update():
    id=int(input("enter id"))
    mark=int(input("enter mark"))
    conn=getconn()
    try:
        conn.execute('UPDATE studinfo SET mark=? where id=?',(mark,id))
        conn.commit()
        print("Data Updated")
        conn.close()
    except Error as e:
        print(e)
def deletedata():
    user_id = input("Enter the ID of the user to delete: ")
    conn = getconn()
    conn.execute('DELETE FROM studinfo WHERE id = ?', (user_id,))
    conn.commit()
    conn.close()
    print(f"\nUser with ID {user_id} deleted successfully.")
def main_menu():
    createtable()
    while True:
        print("\n--- User Management System ---")
        print("1. Add a new user (Create)")
        print("2. View all users (Read)")
        print("3. Update a user (Update)")
        print("4. Delete a user (Delete)")
        print("5. Exit")
        choice = input("Enter your choice (1-5): ")

        if choice == '1':
            adddata()
        elif choice == '2':
            viewdata()
        elif choice == '3':
            update()
        elif choice == '4':
           deletedata()
        elif choice == '5':
            print("Exiting program. Goodbye!")
            break
        else:
            print("Invalid choice. Please enter a number between 1 and 5.")


main_menu()
Program 30:Create a Login form using CGI and display the input on a different page
login_form.py

#!"C: \Users \Asus \AppData \Local \Programs \Python \Python313 \python.exe"

print("Content -Type: text/html \n")

print("""
<html>
<head>
    <title>CGI Login Form</title>
    <style>
        body { font -family: sans -serif; display: flex; justify -content: center; align -items: center;
height: 100vh; background -color: #f0f2f5; }
        form { padding: 2em; border: 1px solid #ccc; border -radius: 8px; background -color: white;
box-shadow: 0 2px 4px rgba(0,0,0,0.1); }
        input[type=text], input[type=password] { width: 100%; padding: 8px; margin -bottom: 10px;
border -radius: 4px; border: 1px solid #ccc; box -sizing: border -box; }
        input[type=submit] { width: 100%; padding: 10px; border: none; border -radius: 4px;
background -color: #007bff; color: white; cursor: pointer; font -size: 16px; }
    </style>
</head>
<body>
    <form method="post" action="/cgi -bin/display_input.py">
        <h2>Login</h2>
        <label for="username">Username:</label><br>
        <input type="text" id="username" name="username" required>
        <br><br>
        <label for="password">Password:</label><br>
        <input type="password" id="password" name="password" required>
        <br><br>
        <input type="submit" value="Log In">
    </form>

</body>
</html>
""")
display_input.py

#!"C: \Users \Asus \AppData \Local \Programs \Python \Python313 \python.exe"

import cgi

print("Content -Type: text/html \n")

form = cgi.FieldStorage()

username_input = form.getvalue("username", "Guest")
password_input = form.getvalue("password", "N/A")

print(f"""
<html>
<head>
    <title>Login Information</title>
     <style>
        body {{ font -family: sans -serif; text -align: center; padding -top: 5em; background -color:
#f0f2f5; }}
        div {{ padding: 2em; border: 1px solid #ccc; border -radius: 8px; background -color: white;
display: inline -block; }}
    </style>
</head>
<body>
    <div>
        <h1>Welcome, {username_input}!</h1>
        <p>Your login details have been received.</p>
        <p><strong>Username entered:</strong> {username_input}</p>
        <p><strong>Password entered:</strong> [Hidden for security]</p>
        <br>
        <a href="/cgi -bin/login_form.py">Go back to Login</a>
    </div>
</body>
</html>
""")

Program 31:Create a registration form for MCA admission and display the inserted data on
#!"C: \Users \Asus \AppData \Local \Programs \Python \Python313 \python.exe"

import cgi
import mysql.connector
from mysql.connector import Error

print("Content -Type: text/html \n")

message = ""
registrations = []
conn = None

try:
    conn = mysql.connector.connect(
        host="localhost",
        user="root",
        password="",
        database="testdb"
    )
    cursor = conn.cursor()

    cursor.execute("""
    CREATE TABLE IF NOT EXISTS mca_admissions (
        id INT AUTO_INCREMENT PRIMARY KEY,
        full_name VARCHAR(255) NOT NULL,
        email VARCHAR(255) NOT NULL,
        previous_degree VARCHAR(255),
        percentage DECIMAL(5, 2)
    )
    """)

    form = cgi.FieldStorage()

    if form.getvalue("full_name") and form.getvalue("email"):
        name = form.getvalue("full_name")
        email = form.getvalue("email")
        degree = form.getvalue("previous_degree")
        percentage = form.getvalue("percentage")

        insert_query = """
        INSERT INTO mca_admissions (full_name, email, previous_degree, percentage)
        VALUES (%s, %s, %s, %s)
        """
        cursor.execute(insert_query, (name, email, degree, percentage))
        conn.commit()
        message = f"Success! {name} has been registered."

    cursor.execute("SELECT id, full_name, email, previous_degree, percentage FROM
mca_admissions")
    registrations = cursor.fetchall()

except Error as e:
    message = f"Database Error: {e}"

finally:
    if conn and conn.is_connected():
        conn.close()

print(f"""
<html>
<head>
    <title>MCA Admission Registration</title>
    <style>
        body {{ font -family: Arial, sans -serif; margin: 2em; background -color: #f4f4f9; }}
        h2 {{ color: #333; }}
        .container {{ display: flex; gap: 4em; }}
        form {{ padding: 1.5em; border: 1px solid #ddd; background -color: #fff; border -radius: 5px;
width: 300px; }}
        input[type=text], input[type=email], input[type=number] {{ width: 100%; padding: 8px;
margin -bottom: 10px; border: 1px solid #ccc; border -radius: 4px; box -sizing: border -box; }}
        input[type=submit] {{ width: 100%; padding: 10px; border: none; border -radius: 4px;
background -color: #28a745; color: white; cursor: pointer; font -size: 16px; }}
        table {{ border -collapse: collapse; width: 100%; background -color: #fff; }}
        th, td {{ border: 1px solid #ddd; padding: 8px; text -align: left; }}
        th {{ background -color: #007bff; color: white; }}
        .message {{ font -weight: bold; color: green; }}
    </style>
</head>
<body>
    <h2>MCA Admission Registration Form</h2>
    <div class="container">
        <div>
            <form method="post" action="/cgi -bin/mca_admission.py">
                <label for="full_name">Name:</label><br>
                <input type="text" id="full_name" name="full_name" required><br>

                <label for="email">Email Address:</label><br>
                <input type="email" id="email" name="email" required><br>

                <label for="previous_degree">Previous Degree:</label><br>
                <input type="text" id="previous_degree" name="previous_degree"><br>

                <label for="percentage">Percentage/CGPA:</label><br>
                <input type="number" id="percentage" name="percentage" step="0.01" min="0"
max="100"><br><br>

                <input type="submit" value="Register">
            </form>
            <p class="message">{message}</p>
        </div>

        <div>
            <h2>Registered Students</h2>
            <table>
                <tr>
                    <th>ID</th>
                    <th>Name</th>
                    <th>Email</th>
                    <th>Previous Degree</th>
                    <th>Percentage</th>
                </tr>
""")

for row in registrations:
    print(f"""
                <tr>
                    <td>{row[0]}</td>
                    <td>{row[1]}</td>
                    <td>{row[2]}</td>
                    <td>{row[3]}</td>
                    <td>{row[4]}</td>
                </tr>
    """)

print("""
            </table>
        </div>
    </div>
</body>
</html>
""")

Program 32:Create a MySQL database and perform INSERT, UPDATE, DESTROY, and SELECT
#!"C: \Users \Asus \AppData \Local \Programs \Python \Python313 \python.exe"

import cgi
import mysql.connector
from mysql.connector import Error

print("Content -Type: text/html \n")

message = ""
records = []
record_to_edit = None
conn = None

try:
    conn = mysql.connector.connect(
        host="localhost",
        user="root",
        password="",
        database="testdb"
    )
    cursor = conn.cursor(dictionary=True)

    cursor.execute("""
    CREATE TABLE IF NOT EXISTS products (
        id INT AUTO_INCREMENT PRIMARY KEY,
        name VARCHAR(255) NOT NULL,
        price DECIMAL(10, 2) NOT NULL
    )
    """)

    form = cgi.FieldStorage()
    action = form.getvalue("action")


    if action == "add":
        name = form.getvalue("name")
        price = form.getvalue("price")
        if name and price:
            cursor.execute ("INSERT INTO products (name, price) VALUES (%s, %s)", (name, price))
            conn.commit()
            message = f"Success: Product '{name}' added."

    elif action == "delete":
        product_id = form.getvalue("id")
        if product_id:
            cursor.execute("DELETE FROM products WHERE id = %s", (product_id,))
            conn.commit()
            message = f"Success: Product ID {product_id} deleted."

    elif action == "edit":
        product_id = form.getvalue("id")
        if product_id:
            cursor.execute("SELECT * FROM products WHERE id = %s", (product_id,))
            record_to_edit = cursor.fetchone()

    elif action == "update":
        product_id = form.getvalue("id")
        name = form.getvalue("name")
        price = form.getvalue("price")
        if product_id and name and price:
            cursor.execute("UPDATE products SET name = %s, price = %s WHERE id = %s", (name,
price, product_id))
            conn.commit()
            message = f"Success : Product ID {product_id} updated."

    cursor.execute("SELECT * FROM products ORDER BY id")
    records = cursor.fetchall()

except Error as e:
    message = f"Database Error: {e}"

finally:
    if conn and conn.is_connected():
        conn.close()

print(f"""
<html>
<head>
    <title>MySQL CRUD Interface</title>
    <style>
        body {{ font -family: Arial, sans -serif; margin: 2em; }}
        .container {{ display: grid; grid -template -columns: 350px 1fr; gap: 2em; }}
        form {{ padding: 1.5em; border: 1px solid #ddd; background -color: #f9f9f9; border -radius:
5px; }}
        table {{ border -collapse: collapse; width: 100%; }}
        th, td {{ border: 1px solid #ddd; padding: 8px; text -align: left; }}
        th {{ background -color: #f2f2f2; }}
        .message {{ font -weight: bold; margin -bottom: 1em; }}
        .edit -form {{ background -color: #fffbe6; border -color: #ffc107; }}
        .action -form {{ display: inline; }}
        .action -btn {{ padding: 5px 10px; border: none; border -radius: 4px; color: white; cursor:
pointer; }}
        .edit -btn {{ background -color: #ffc107; }}
        .delete -btn {{ background -color: #dc3545; }}
    </style>
</head>
<body>
    <h1>Product Management</h1>
    <p class="message">{message}</p>
    <div class="container">
        <div>
""")

if record_to_edit:
    print(f"""
            <form class="edit -form" method="post" action="/cgi -bin/crud_mysql.py">
                <h3>Edit Product ID: {record_to_edit['id']}</h3>
                <input type="hidden" name="action" value="update">
                <input type="hidden" name="id" value="{record_to_edit['id']}">
                <label>Name:</label><br>
                <input type="text" name="name" value="{record_to_edit['name']}" required><br><br>
                <label>Price:</label><br>
                <input type="number" name="price" step="0.01" value="{record_to_edit['price']}"
required><br><br>
                <input type="submit" value="Update Product">
            </form>
    """)
else:
    print("""
            <form method="post" action="/cgi -bin/crud_mysql.py">
                <h3>Add New Product</h3>
                <input type="hidden" name="action" value="add">
                <label>Name:</label><br>
                <input type="text" name="name" required><br><br>
                <label>Price:</label><br>
                <input type="number" name="price" step="0.01" required><br><br>
                <input type="submit" value="Add Product">
            </form>
    """)

print("""
        </div>
        <div>
            <h2>Product List</h2>
            <table>
                <tr>
                    <th>ID</th>
                    <th>Name</th>
                    <th>Price</th>
                    <th>Actions</th>
                </tr>
""")

for record in records:
    print(f"""
                <tr>
                    <td>{record['id']}</td>
                    <td>{record['name']}</td>
                    <td>${record['price']:.2f}</td>
                    <td>
                        <form class="action -form" method="post" action="/cgi -bin/crud_mysql.py">
                            <input type="hidden" name="action" value="edit">
                            <input type="hidden" name="id" value="{record['id']}">
                            <button type="submit" class="action -btn edit -btn">Edit</button>
                        </form>
                        <form class="action -form" method="post" action="/cgi -bin/crud_mysql.py">
                            <input type="hidden" name="action" value="delete">
                            <input type="hidden" name="id" value="{record['id']}">
                            <button type="submit" class="action -btn delete -btn">Delete</button>
                        </form>
                    </td>
                </tr>
    """)

print("""
            </table>
        </div>
    </div>
</body>
</html>
""")

Program 33:Create a numpy array filled with all ones by defining its shape
import numpy as np
# Define the shape of the array
array_shape = (3, 4)

# Create a NumPy array filled with ones
ones_array = np.ones(array_shape)

print(f"NumPy array of shape {array_shape} filled with ones:")
print(ones_array)

Program 34:How do you remove rows from a Numpy array that contains non -numeric
import numpy as np

data = np.array([[1, 2, 3],
                 [4, 'abc', 6],
                 [7, 8, 9],
                 ['def', 10, 11]])

print("Original array:")
print(data)
numeric_rows = []
for row in data:
    is_numeric_row = True
    for item in row:
        try:
            float(item)
        except ValueError:
            is_numeric_row = False
            break

    if is_numeric_row:
        numeric_rows.append(row)

# Convert the list of numeric rows back to a NumPy array
cleaned_array = np.array(numeric_rows)

print(" \nArray after removing rows with non -numeric values:")
print(cleaned_array)

Program 35:Remove single -dimensional entries from the shape of an array
import numpy as np

data = np.array([[[1, 2, 3]], [[4, 5, 6]]])

print("Original array shape:", data.shape)

# Remove single -dimensional entries
squeezed_array = np.squeeze(data)
print("Squeezed array shape:", squeezed_array.shape)
print("Squeezed array: \n", squeezed_array)

Program 36:How do you check whether specified values are present in the NumPy array?
import numpy as np

data = np.array([10, 20, 30, 40, 50, 60])
# Values to check for presence
values_to_check = [20, 55, 40]

print("Original array:", data)
print("Values to check:", values_to_check)

# Method 1: Using boolean indexing
print(" \nMethod 1: Using boolean indexing")
for value in values_to_check:
    is_present = (data == value).any()
    print(f"Is {value} present? {is_present}")

# Method 2: Using np.isin()
print(" \nMethod 2: Using np.isin()")
presence_mask = np.isin(data, values_to_check)
print("Presence mask:", presence_mask)


# To check if *any* of the values are present:
print(f"Are any of the values present? {presence_mask.any()}")
print(f"Are all of the values present? {np.all(np.isin(values_to_check, data))}")

Program 37:Write a NumPy program to sort a given array of shape 2 along the first axis, last
import numpy as np
data = np.array([[3, 1, 2],
                 [6, 5, 4]])

print("Original array:")
print(data)

# Sort along the first axis (rows)
sorted_axis_0 = np.sort(data, axis=0)
print(" \nSorted along the first axis (axis=0):")
print(sorted_axis_0)

# Sort along the last axis (columns)
sorted_axis_1 = np.sort(data, axis=1)
print(" \nSorted along the last axis (axis=1):")
print(sorted_axis_1)

# Sort the flattened array

sorted_flattened = np.sort(data.flatten())
print(" \nSorted flattened array:")
print(sorted_flattened)

Program 38:Write a NumPy program to create a structured array from a given student name,
import numpy as np

student_data = [
    ('Alice', 1.65, 10),
    ('Bob', 1.80, 11),
    ('Charlie', 1.75, 10),
    ('David', 1.70, 11),
    ('Eve', 1.60, 10)
]
# Define the data type for the structured array
data_type = [('name', 'S10'), ('height', 'f4'), ('class', 'i4')]

# Create the structured array
structured_array = np.array(student_data, dtype=data_type)

print("Original structured array:")
print(structured_array)


# Sort by class, then by height
sorted_array = np.sort(structured_array, order=['class', 'height'])

print(" \nSorted structured array (by class, then height):")
print(sorted_array)

Program 39:Write a NumPy program to sort a given complex array using the real part first,
import numpy as np
# Complex NumPy array
complex_array = np.array([3 + 2j, 1 + 4j, 2 + 1j, 3 + 1j, 1 + 2j])
print("Original complex array:")
print(complex_array)
# Sort the complex array by real part, then imaginary part
sorted_complex_array = np.sort(complex_array)
print(" \nSorted complex array (by real then imaginary part):")
print(sorted_complex_array)

Program 40:Write a NumPy program to sort a given array by the nth column
import numpy as np
data = np.array([[3, 2, 1],
                 [6, 5, 4],
                 [9, 8, 7]])
print("Original array:")
print(data)
n = 1
sorted_indices = np.argsort(data[:, n])
sorted_array_by_column = data[sorted_indices]
print(f" \nSorted array by column {n}:")
print(sorted_array_by_column)

Program 41:Calculate the sum of the diagonal elements of a NumPy array
import numpy as np
data = np.array([[1, 2, 3],
                 [4, 5, 6],
                 [7, 8, 9]])
print("Original array:")
print(data)
# Calculate the sum of the diagonal elements
diagonal_sum = np.trace(data)
print(f" \nSum of diagonal elements: {diagonal_sum}")

Program 42:Write a program for Matrix Multiplication in NumPy
import numpy as np
# Define two matrices
matrix1 = np.array([[1, 2],
                    [3, 4]])
matrix2 = np.array([[5, 6],
                    [7, 8]])
print("Matrix 1:")
print(matrix1)
print(" \nMatrix 2:")
print(matrix2)
# matrix multiplication
result_matrix = np.dot(matrix1, matrix2)
print(" \nResult of Matrix Multiplication (Matrix 1 @ Matrix 2):")
print(result_matrix)

Program 43:Multiply matrices of complex numbers using NumPy in Python
import numpy as np
# Define two matrices with complex numbers
complex_matrix1 = np.array([[1 + 2j, 3 + 4j],
                            [5 + 6j, 7 + 8j]])

complex_matrix2 = np.array([[9 + 10j, 11 + 12j],
                            [13 + 14j, 15 + 16j]])

print("Complex Matrix 1:")
print(complex_matrix1)
print(" \nComplex Matrix 2:")
print(complex_matrix2)

# Perform matrix multiplication with complex numbers
complex_result_matrix = complex_matrix1 @ complex_matrix2
# Alternative: complex_result_matrix = np.dot(complex_matrix1, complex_matrix2)

print(" \nResult of Complex Matrix Multiplication (Complex Matrix 1 @ Complex Matrix 2):")

print(complex_result_matrix)

Program 44:Compute the covariance matrix of two given NumPy arrays.
import numpy as np

x = np.array([1, 2, 3, 4, 5])
y = np.array([5, 4, 3, 2, 1])
print("Array x:", x)
print("Array y:", y)
covariance_matrix = np.cov(x, y)
print(" \nCovariance matrix of x and y:")
print(covariance_matrix)

Program 45:Convert covariance matrix to correlation matrix using Python
import numpy as np
covariance_matrix = np.array([[ 2.5, -2.5],
                              [-2.5,  2.5]])
print("Original Covariance Matrix:")
print(covariance_matrix)
std_devs = np.sqrt(np.diag(covariance_matrix))
outer_std_devs = np.outer(std_devs, std_devs)
correlation_matrix = np.divide(covariance_matrix, outer_std_devs)
print(" \nCorrelation Matrix:")
print(correlation_matrix)
x = np.array([1, 2, 3, 4, 5])
y = np.array([5, 4, 3, 2, 1])
correlation_matrix_from_data = np.corrcoef(x, y)
print(" \nCorrelation Matrix computed directly from data (for comparison):")
print(correlation_matrix_from_data)

Program 46:Write a NumPy program to compute the histogram of nums against the bins
import numpy as np
nums = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
bins = np.array([0, 2, 4, 6, 8, 10])

print("Data:", nums)
print("Bins:", bins)
histogram, bin_edges = np.histogram(nums, bins)
print(" \nHistogram (counts per bin):", histogram)
print("Bin edges:", bin_edges)

Program 47:Write a NumPy program to compute the cross -correlation of two given arrays
import numpy as np
x = np.array([1, 2, 3, 4, 5])
y = np.array([6, 7, 8, 9, 10])
print("Array x:", x)
print("Array y:", y)
cross_correlation = np.correlate(x, y, mode='full')
print(" \nCross -correlation of x and y (mode='full'):")
print(cross_correlation)
cross_correlation_valid = np.correlate(x, y, mode='valid')
print(" \nCross -correlation of x and y (mode='valid'):")
print(cross_correlation_valid)
cross_correlation_same = np.correlate(x, y, mode='same')
print(" \nCross -correlation of x and y (mode='same'):")
print(cross_correlation_same)

Program 48:Write a NumPy program to compute the mean, standard deviation, and variance
import numpy as np
data = np.array([[1, 2, 3, 4],
                 [5, 6, 7, 8],
                 [9, 10, 11, 12]])
print("Original array:")
print(data)
mean_along_axis_1 = np.mean(data, axis=1)
print(" \nMean along the second axis (axis=1):", mean_along_axis_1)
std_dev_along_axis_1 = np.std(data, axis=1)
print("Standard deviation along the second axis (axis=1):", std_dev_along_axis_1)
variance_along_axis_1 = np.var(data, axis=1)
print("Variance along the second axis (axis=1):", variance_along_axis_1)

Program 49:Visualize the following using the given dataset - alphabet_stock_data.csv
import pandas as pd
import matplotlib.pyplot as plt
try:
    df = pd.read_csv('Alphabet Stock.csv')
except FileNotFoundError:
    print("Error: 'Alphabet Stock.csv' not found. Please ensure the file is in the correct directory.")
    exit()
df['Date'] = pd.to_datetime(df['Date'])
df.set_index('Date', inplace=True)
start_date = '2020 -01-01'
end_date = '2020 -10-22'

df_range = df.loc[start_date:end_date]


if df_range.empty:
    print(f"No data available for the selected date range: {start_date} to {end_date}.")
else:
    fig, axs = plt.subplots(2, 2, figsize=(20, 14))
    fig.suptitle(f'Alphabet Inc. Stock Analysis ({start_date} to {end_date})', fontsize=20)

    axs[0, 0].plot(df_range.index, df_range['Close'], color='blue', label='Close Price')
    axs[0, 0].set_title('Historical Stock Prices')
    axs[0, 0].set_xlabel('Date')
    axs[0, 0].set_ylabel('Stock Price (USD)')
    axs[0, 0].grid(True)
    axs[0, 0].tick_params(axis='x', rotation=45)
    axs[0, 0].legend()

    axs[0, 1].bar(df_range.index, df_range['Volume'], color='green', alpha=0.7)
    axs[0, 1].set_title('Trading Volume')
    axs[0, 1].set_xlabel('Date')
    axs[0, 1].set_ylabel('Volume')
    axs[0, 1].grid(axis='y')
    axs[0, 1].tick_params(axis='x', rotation=45)

    prices = [df_range['Open'], df_range['High'], df_range['Low'], df_range['Close']]
    labels = ['Open', 'High', 'Low', 'Close']
    axs[1, 0].hist(prices, bins=50, stacked=True, label=labels, edgecolor='black')
    axs[1, 0].set_title('Stacked Histogram of OHLC Prices')
    axs[1, 0].set_xlabel('Stock Price (USD)')
    axs[1, 0].set_ylabel('Frequency')
    axs[1, 0].legend()
    axs[1, 0].grid(axis='y')

    axs[1, 1].scatter(df_range['Close'], df_range['Volume'], alpha=0.6, edgecolors='w', s=50)
    axs[1, 1].set_title('Trading Volume vs. Stock Price')
    axs[1, 1].set_xlabel('Stock Price (USD)')
    axs[1, 1].set_ylabel('Volume')
    axs[1, 1].grid(True)

    plt.tight_layout(rect=[0, 0, 1, 0.96])
    plt.show()

Program 50:Handle the given datasets with adequate preprocessing steps mentioned and
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.preprocessing import StandardScaler, MinMaxScaler, LabelEncoder

sns.set_style("whitegrid")

def preprocess_and_visualize_titanic(df):
    df['Age'] = df['Age'].fillna(df['Age'].median())
    df['Embarked'] = df['Embarked'].fillna(df['Embarked'].mode()[0])
    df.drop(columns=['Cabin', 'PassengerId', 'Name', 'Ticket'], inplace=True)


    df = pd.get_dummies(df, columns=['Sex', 'Embarked'], drop_first=True)

    X = df.drop('Survived', axis=1)
    y = df['Survived']

    scaler = MinMaxScaler()
    X_scaled = scaler.fit_transform(X)
    X_scaled = pd.DataFrame(X_scaled, columns=X.columns)

    fig, axes = plt.subplots(2, 2, figsize=(16, 12))
    fig.suptitle('Titanic Dataset Analysis', fontsize=20)

    sns.countplot(ax=axes[0, 0], x='Survived', data=df)
    axes[0, 0].set_title('Survival Count (0 = No, 1 = Yes)')

    sns.countplot(ax=axes[0, 1], x='Sex_male', data=df, hue='Survived')
    axes[0, 1].set_title('Survival by Gender (0 = Female, 1 = Male)')
    axes[0, 1].set_xlabel('Gender')

    sns.countplot(ax=axes[1, 0], x='Pclass', data=df, hue='Survived')
    axes[1, 0].set_title('Survival Count by Passenger Class')

    sns.histplot(ax=axes[1, 1], data=df, x='Age', kde=True, bins=30)
    axes[1, 1].set_title('Age Distribution of Passengers')

    plt.tight_layout(rect=[0, 0, 1, 0.96])
    plt.show()

def preprocess_and_visualize_diabetes(df):
    cols_to_replace = ['Glucose', 'BloodPressure', 'SkinThickness', 'Insulin', 'BMI']
    for col in cols_to_replace:
        df[col] = df[col].replace(0, np.nan)
        mean_val = df[col].mean()
        df[col] = df[col].fillna(mean_val)

    X = df.drop('Outcome', axis=1)
    y = df['Outcome']

    scaler = StandardScaler()
    X_scaled = scaler.fit_transform(X)
    X_scaled = pd.DataFrame(X_scaled, columns=X.columns)

    fig, axes = plt.subplots(2, 2, figsize=(16, 12))
    fig.suptitle('Diabetes Dataset Analysis', fontsize=20)

    sns.countplot(ax=axes[0, 0], x='Outcome', data=df)
    axes[0, 0].set_title('Diabetes Outcome (0 = No, 1 = Yes)')

    sns.histplot(ax=axes[0, 1], data=df, x='Glucose', hue='Outcome', kde=True)
    axes[0, 1].set_title('Glucose Distribution by Outcome')

    sns.boxplot(ax=axes[1, 0], x='Outcome', y='BMI', data=df)
    axes[1, 0].set_title('BMI Distribution by Outcome')

    sns.histplot(ax=axes[1, 1], data=df, x='Age', kde=True, bins=30)
    axes[1, 1].set_title('Age Distribution of Patients')

    plt.tight_layout(rect=[0, 0, 1, 0.96])
    plt.show()

def preprocess_and_visualize_breast_cancer(df):
    if 'Unnamed: 32' in df.columns:
        df = df.drop(columns=['id', 'Unnamed: 32'])
    else:
        df = df.drop(columns=['id'])

    le = LabelEncoder()
    df['diagnosis'] = le.fit_transform(df['diagnosis']) # M=1, B=0

    X = df.drop('diagnosis', axis=1)
    y = df['diagnosis']

    scaler = StandardScaler()
    X_scaled = scaler.fit_transform(X)
    X_scaled = pd.DataFrame(X_scaled, columns=X.columns)

    fig, axes = plt.subplots(1, 2, figsize=(16, 6))
    fig.suptitle('Breast Cancer Dataset Analysis', fontsize=20)

    sns.countplot(ax=axes[0], x='diagnosis', data=df)
    axes[0].set_title('Diagnosis Count (0 = Benign, 1 = Malignant)')

    mean_features = ['diagnosis'] + list(df.columns[1:11])
    corr_matrix = df[mean_features].corr()
    sns.heatmap(ax=axes[1], data=corr_matrix, annot=False, cmap='coolwarm')
    axes[1].set_title('Correlation Heatmap of Mean Features')

    plt.tight_layout(rect=[0, 0, 1, 0.96])
    plt.show()

    fig, axes = plt.subplots(1, 2, figsize=(16, 6))
    sns.violinplot(ax=axes[0], x='diagnosis', y='radius_mean', data=df)
    axes[0].set_title('Radius Mean Distribution by Diagnosis')
    sns.violinplot(ax=axes[1], x='diagnosis', y='texture_mean', data=df)
    axes[1].set_title('Texture Mean Distribution by Diagnosis')
    plt.show()


if __name__ == '__main__':
    try:
        titanic_df = pd.read_csv('Titanic -Dataset.csv')
        preprocess_and_visualize_titanic(titanic_df.copy())
    except FileNotFoundError:
        print("Error: 'Titanic -Dataset.csv' not found.")

    try:
        diabetes_df = pd.read_csv('diabetes.csv')
        preprocess_and_visualize_diabetes(diabetes_df.copy())
    except FileNotFoundError:
        print("Error: 'diabetes.csv' not found.")

    try:
        cancer_df = pd.read_csv('data.csv')
        preprocess_and_visualize_breast_cancer(cancer_df.copy())
    except FileNotFoundError:
        print("Error: 'data.csv' not found.")

Program 51:Evaluate the dataset (User_Data.csv) and predict whether a user will purchase
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler, LabelEncoder
from sklearn.linear_model import LogisticRegression
from sklearn.neighbors import KNeighborsClassifier
from sklearn.svm import SVC
from sklearn.metrics import accuracy_score, classification_report, confusion_matrix
from matplotlib.colors import ListedColormap

try:
    df = pd.read_csv('User_Data.csv')
except FileNotFoundError:
    print("Error: 'User_Data.csv' not found. Please ensure the file is in the correct directory.")
    exit()


df = df.drop('User ID', axis=1)

le = LabelEncoder()
df['Gender'] = le.fit_transform(df['Gender'])

X = df[['Gender', 'Age', 'EstimatedSalary']]
y = df['Purchased']

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.25, random_state=42)

scaler = StandardScaler()
X_train_scaled = scaler.fit_transform(X_train)
X_test_scaled = scaler.transform(X_test)

models = {
    "Logistic Regression": LogisticRegression(random_state=42),
    "K-Nearest Neighbors (KNN)": KNeighborsClassifier(n_neighbors=5),
    "Support Vector Machine (SVM)": SVC(kernel='rbf', random_state=42)
}

print(" --- Model Performance Comparison ---\n")
for name, model in models.items():
    model.fit(X_train_scaled, y_train)

    y_pred = model.predict(X_test_scaled)

    accuracy = accuracy_score(y_test, y_pred)
    report = classification_report(y_test, y_pred)

    print(f" --- {name} ---")
    print(f"Accuracy: {accuracy:.4f}")
    print("Classification Report:")
    print(report)
    print("Confusion Matrix:")
    print(confusion_matrix(y_test, y_pred))
    print(" -" * 30 + " \n")

X_vis = df[['Age', 'EstimatedSalary']]
y_vis = df['Purchased']

X_train_vis, X_test_vis, y_train_vis, y_test_vis = train_test_split(X_vis, y_vis, test_size=0.25,
random_state=42)
scaler_vis = StandardScaler()
X_train_vis_scaled = scaler_vis.fit_transform(X_train_vis)
X_test_vis_scaled = scaler_vis.transform(X_test_vis)

models_vis = {
    "Logistic Regression": LogisticRegression(random_state=42),
    "K-Nearest Neighbors (KNN)": KNeighborsClassifier(n_neighbors=5),
    "Support Vector Machine (SVM)": SVC(kernel='rbf', random_state=42)
}
for name, model in models_vis.items():
    model.fit(X_train_vis_scaled, y_train_vis)

fig, axes = plt.subplots(1, 3, figsize=(20, 6))
fig.suptitle('Classifier Decision Boundaries (Test Set)', fontsize=16)

cmap_light = ListedColormap(['#FFAAAA', '#AAFFAA'])
cmap_bold = ListedColormap(['#FF0000', '#00FF00'])

X_set, y_set = X_test_vis_scaled, y_test_vis
X1, X2 = np.meshgrid(np.arange(start=X_set[:, 0].min() - 1, stop=X_set[:, 0].max() + 1,
step=0.01),
                     np.arange(start=X_set[:, 1].min() - 1, stop=X_set[:, 1].max() + 1, step=0.01))

for i, (name, model) in enumerate(models_vis.items()):
    ax = axes[i]

    Z = model.predict(np.array([X1.ravel(), X2.ravel()]).T)
    Z = Z.reshape(X1.shape)
    ax.contourf(X1, X2, Z, alpha=0.75, cmap=cmap_light)

    for j, val in enumerate(np.unique(y_set)):
        ax.scatter(X_set[y_set == val, 0], X_set[y_set == val, 1],
                   c=[cmap_bold(j)], label=f'Purchased = {val}')

    ax.set_title(name)
    ax.set_xlabel('Scaled Age')
    ax.set_ylabel('Scaled Estimated Salary')
    ax.legend()

plt.tight_layout(rect=[0, 0, 1, 0.96])
plt.show()

Program 52:A Comparative Study of Classification Algorithms on Real -World Data
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import os
from sklearn.model_selection import train_test_split, GridSearchCV
from sklearn.preprocessing import StandardScaler
from sklearn.linear_model import LogisticRegression
from sklearn.tree import DecisionTreeClassifier, plot_tree
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score, confusion_matrix, classification_report,
roc_auc_score, roc_curve, precision_recall_curve, auc
import warnings
warnings.filterwarnings('ignore')
os.makedirs('plots', exist_ok=True)
csv_path = 'healthcare -dataset -stroke -data.csv'

if not os.path.exists(csv_path):
    raise FileNotFoundError(f"{csv_path} not found. Please upload it to the runtime or change
csv_path.")

df = pd.read_csv(csv_path)
print('Dataset loaded:', csv_path)
df.head()
print('Shape:', df.shape)
print(' \nInfo:')
print(df.info())
display(df.describe(include='all'))
print(' \nMissing values per column: \n', df.isnull().sum())
print(' \nNumber of duplicate rows:', df.duplicated().sum())
print(' \nStroke value counts: \n', df['stroke'].value_counts())
data = df.copy()

if 'id' in data.columns:
    data = data.drop(columns=['id'])
if 'bmi' in data.columns:
    median_bmi = data['bmi'].median()
    data['bmi'] = data['bmi'].fillna(median_bmi)
    print('Filled bmi NA with median:', median_bmi)

dups = data.duplicated().sum()
print('Duplicate rows before removal:', dups)
data = data.drop_duplicates()
print('Duplicate rows after removal:', data.duplicated().sum())

categorical_cols = ['gender','ever_married','work_type','Residence_type','smoking_status']
existing_cats = [c for c in categorical_cols if c in data.columns]
data_encoded = pd.get_dummies(data, columns=existing_cats, drop_first=True)
print(' \nColumns after encoding:', data_encoded.columns.tolist())

X = data_encoded.drop('stroke', axis=1)
y = data_encoded['stroke']

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42, stratify=y)
print(' \nTrain shape:', X_train.shape, 'Test shape:', X_test.shape)

num_cols = [c for c in ['age','avg_glucose_level','bmi','hypertension','heart_disease'] if c in
X_train.columns]
scaler = StandardScaler()
X_train[num_cols] = scaler.fit_transform(X_train[num_cols])
X_test[num_cols] = scaler.transform(X_test[num_cols])
print(' \nNumeric columns scaled:', num_cols)

plt.figure(figsize=(6,4))
sns.countplot(x='stroke', data=data)
plt.title('Stroke Count (0 = No, 1 = Yes)')
plt.savefig('plots/stroke_count.png', bbox_inches='tight')
plt.show()
num_features = [c for c in ['age','avg_glucose_level','bmi'] if c in data.columns]
data[num_features].hist(figsize=(12,4), bins=20)
plt.suptitle('Histograms of numeric features')
plt.savefig('plots/histograms.png', bbox_inches='tight')
plt.show()
plt.figure(figsize=(10,5))
sns.boxplot(data=data[num_features])
plt.title('Boxplots of numeric features')
plt.savefig('plots/boxplots.png', bbox_inches='tight')
plt.show()

corr = data_encoded.corr()
plt.figure(figsize=(14,10))
sns.heatmap(corr, cmap='coolwarm', vmax=0.6)
plt.title('Correlation heatmap (encoded features)')
plt.savefig('plots/corr_heatmap.png', bbox_inches='tight')
plt.show()
logreg = LogisticRegression(max_iter=1000, random_state=42)
logreg.fit(X_train, y_train)
y_pred_lr = logreg.predict(X_test)
y_prob_lr = logreg.predict_proba(X_test)[:,1]

dt = DecisionTreeClassifier(random_state=42)
dt.fit( X_train, y_train)
y_pred_dt = dt.predict(X_test)
y_prob_dt = dt.predict_proba(X_test)[:,1]

rf = RandomForestClassifier(n_estimators=100, random_state=42)
rf.fit(X_train, y_train)
y_pred_rf = rf.predict(X_test)
y_prob_rf = rf.predict_proba(X_test)[:,1]

def eval_model(y_true, y_pred, y_prob, model_name):
    acc = accuracy_score(y_true, y_pred)
    auc_score = roc_auc_score(y_true, y_prob)
    print(f" --- {model_name} ---")
    print('Accuracy:', acc)
    print('ROC AUC:', auc_score)
    print('Confusion Matrix: \n', confusion_matrix(y_true, y_pred))
    print(' \nClassification Report: \n', classification_report(y_true, y_pred))
    fpr, tpr, _ = roc_curve(y_true, y_prob)
    plt.figure(figsize=(6,5))
    plt.plot(fpr, tpr, label=f'{model_name} (AUC = {auc_score:.2f})')
    plt.plot([0,1],[0,1],'k --')
    plt.xlabel('False Positive Rate'); plt.ylabel('True Positive Rate'); plt.title(f'ROC Curve -
{model_name}')
    plt.legend()
    plt.savefig(f'plots/roc_{model_name}.png', bbox_inches='tight')
    plt.show()

eval_model(y_test, y_pred_lr, y_prob_lr, 'Logistic_Regression')
eval_model(y_test, y_pred_dt, y_prob_dt, 'Decision_Tree')
eval_model(y_test, y_pred_rf, y_prob_rf, 'Random_Forest')
prec, rec, _ = precision_recall_curve(y_test, y_prob_rf)
pr_auc = auc(rec, prec)
plt.figure(figsize=(6,5))
plt.plot(rec, prec, label=f'RandomForest PR AUC = {pr_auc:.2f}')
plt.xlabel('Recall'); plt.ylabel('Precision'); plt.title('Precision -Recall Curve - Random Forest')
plt.legend()
plt.savefig('plots/pr_random_forest.png', bbox_inches='tight')
plt.show()

importances = pd.Series(rf.feature_importances_,
index=X_train.columns).sort_values(ascending=False).head(20)
plt.figure(figsize=(8,6))
sns.barplot(x=importances.values, y=importances.index)
plt.title('Top 20 Feature Importances (Random Forest)')
plt.savefig('plots/feature_importances_rf.png', bbox_inches='tight')
plt.show()

program 59 titanic

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler,LabelEncoder
from sklearn.neighbors import KNeighborsClassifier
from sklearn.linear_model import LogisticRegression
from sklearn.tree import DecisionTreeClassifier
from sklearn.ensemble import RandomForestClassifier
from sklearn.svm import SVC
from sklearn.metrics import accuracy_score,classification_report,confusion_matrix
#impoer and read data
try:
    df=pd.read_csv("Titanic-Dataset.csv")
except FileNotFoundError:
    print("file not found")
df.head()
print(df.shape)
print(df.isnull().sum())
df.info()


#cleaning data
df=df.drop(columns=['Cabin', 'PassengerId', 'Name', 'Ticket'])
df['Age']=df['Age'].fillna(df['Age'].median())
df['Embarked']=df['Embarked'].fillna(df['Embarked'].mode()[0])
#df.drop_duplicate(inplace=true)
df = pd.get_dummies(df, drop_first=True)


# label=LabelEncoder()
# df['Sex']=label.fit_transform(df['Sex'])
x=df.drop(columns=['Survived'])
y=df['Survived']

x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.25,random_state=42)

scaler=StandardScaler()
x_train_scaled=scaler.fit_transform(x_train)
x_test_scaled=scaler.fit_transform(x_test)

model={"LogisticRegression":LogisticRegression(random_state=42),
       "DecisionTree":DecisionTreeClassifier(random_state=42),
       "Random forest":RandomForestClassifier(random_state=42),
       "KNN":KNeighborsClassifier(n_neighbors=5),
       "SVM":SVC(probability=True)
      }

for name,model in model.items():
    model.fit(x_train_scaled,y_train)
    y_pred=model.predict(x_test_scaled)
    accuracy=accuracy_score(y_pred,y_test)
    print(f"{name}")
    print(f"Accuracy:{accuracy:.4f}")
    print("Report")
    print(classification_report(y_pred,y_test))
    print("con matrix")
    print(confusion_matrix(y_pred,y_test))


sns.countplot(x=y)
plt.title("Target Variable Distribution")
plt.show()

sns.histplot(df['Age'])
plt.show()

sns.boxplot(y=df['Age'])
plt.show()

sns.scatterplot(x='Age',y='Fare',data=df)
plt.show()

sns.lineplot(x=df.index[:50],y=df['Fare'][:50])
plt.show()

sns.heatmap(df.corr(),annot=True)
plt.show()
