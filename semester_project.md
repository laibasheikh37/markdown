# Student Performance Tracker

## Project Overview

The **Student Performance Tracker** is a Python application that allows teachers to manage and track the performance of students in various subjects. This program enables teachers to input student names, scores in multiple subjects (Math, Science, English), calculate individual student averages, check whether they are passing or failing, and calculate the overall class average.

This project demonstrates the use of Object-Oriented Programming (OOP) concepts and data structures like dictionaries to manage students' information efficiently.

## Features

- **Add Students**: Enter student names and scores for multiple subjects.
- **Calculate Student Average**: Compute the average score for each student across subjects.
- **Pass/Fail Check**: Determine if the student is passing based on their individual scores (passing grade threshold is 40).
- **Class Average**: Calculate and display the average score for the entire class.
- **Error Handling**: Proper handling for invalid inputs, ensuring scores are within a valid range (0-100) and that only valid integers are entered.

## Technologies Used

- Python 3.x
- Object-Oriented Programming (OOP)
- Data Structures: Lists and Dictionaries

## Requirements

- Python 3.x installed on your system.
- No external libraries or dependencies are required.

## How to Use

1. Clone or download the repository to your local machine.

   ```bash
   git clone https://github.com/yourusername/student-performance-tracker.git
   
2. Navigate to the project directory.
   cd student-performance-tracker
3. Run the Python script
     python student_performance_tracker.py
 
4. Follow the on-screen prompts to input student names and their scores for subjects (Math, Science, English).

5. Once you finish entering all students' data, the program will display each student's performance (average score and pass/fail status) along with the overall class average.

## Example Output
Enter the student's name (or type 'exit' to stop): John Doe
Enter John's score in Math: 75
Enter John's score in Science: 85
Enter John's score in English: 90
Enter the student's name (or type 'exit' to stop): Jane Smith
Enter Jane's score in Math: 40
Enter Jane's score in Science: 50
Enter Jane's score in English: 30
Enter the student's name (or type 'exit' to stop): exit

Student: John Doe
Average Score: 83.33
Status: Passing

Student: Jane Smith
Average Score: 40.00
Status: Failing
Class Average: 61.67

## Code Structure
1.Student Class
- Attributes:
name: The student's name (string).
scores: A dictionary of subjects and their corresponding scores.
- Methods:
add_score(subject, score): Adds a score for a subject.
calculate_average(): Calculates the student's average score.
is_passing(): Checks if the student is passing (i.e., all subject scores are greater than or equal to 40).
display_performance(): Displays the student's name, average score, and pass/fail status.
## PerformanceTracker Class
- Attributes:
students: A dictionary that stores student names as keys and Student objects as values.
- Methods:
  - add_student(name, scores): Adds a student and their scores to the tracker.
  - calculate_class_average(): Calculates the average score of the entire class.
 - display_all_performance(): Displays the performance of all students in the tracker.
## Main Program Flow
 The main program flow:

- Prompts the user to enter student names and scores for each subject.
- Calls methods to add students to the tracker.
- Displays individual student performance and the class average.

