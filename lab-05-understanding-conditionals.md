Lab 5: Understanding Conditionals (if, elif, else)
🧠 What I Learned

In this lab, I learned how to control program flow in Python using conditional statements such as if, elif, and else. I practiced evaluating user input and applying multiple conditions to make logical decisions. This lab helped me understand how Python executes code blocks based on conditions.

🎯 Lab Objectives

Understand how to implement conditional logic using if, elif, and else

Learn how to handle multiple conditions efficiently

Practice classifying user input using conditional statements

🧪 Lab Tasks Performed
🔹 Task 1: User Input and Number Classification

Objective:
Determine whether a number entered by the user is positive, negative, or zero.

Step 1: Prompt User Input

The program asks the user to enter a number:

number = float(input("Enter a number: "))

Step 2: Classify the Number Using Conditionals
if number > 0:
    print("Positive")
elif number < 0:
    print("Negative")
else:
    print("Zero")

🔍 Explanation

if checks whether the number is greater than zero

elif checks whether the number is less than zero

else runs if neither condition is true (number is zero)

🔹 Task 2: Exploring Multiple Conditions with elif

Objective:
Understand how elif allows checking multiple conditions sequentially.

Step 1: Grading System Example
score = int(input("Enter your score: "))

if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
elif score >= 60:
    print("Grade: D")
else:
    print("Grade: F")

🔍 Explanation

elif stands for else if

Conditions are checked from top to bottom

Once a condition is true, remaining conditions are skipped

Ideal for mutually exclusive conditions like grading systems

🧩 Key Concepts

if statement: Executes code when a condition is true

elif statement: Checks additional conditions if previous ones are false

else statement: Executes when no conditions are met

Program flow control: Determines which part of code runs based on logic

Summary

In this lab, I successfully:

Used conditional statements to classify numbers

Implemented multiple condition checks using elif

Understood how Python evaluates conditions sequentially

Applied conditionals to real-world scenarios like grading systems

Mastering conditionals is essential for building intelligent programs that respond dynamically to user input.
