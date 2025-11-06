# pseudocode.py
student-grade-tracker
# Student Grade Tracker
# This program uses parallel arrays, a nested loop, and a function
# to calculate and display the average grade for each student.

# Function to calculate average
def calculate_average(grades):
    total = 0
    for grade in grades:
        total += grade
    average = total / len(grades)
    return average

# Parallel arrays
students = ["Jessica", "karina", "xavier"]
grades = [
    [90, 85, 88],  # Jessica
    [78, 82, 80],  # Karin
    [92, 94, 89]   # Xavier
]

# Nested loop: outer for students, inner for grades
for i in range(len(students)):
    print(f"\nGrades for {students[i]}:")
    for j in range(len(grades[i])):
        print(f"  Subject {j + 1} grade: {grades[i][j]}")
    avg = calculate_average(grades[i])
    print(f"{students[i]}'s average grade: {avg:.2f}")



