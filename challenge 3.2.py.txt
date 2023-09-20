
def sort_students(students):
    students.sort(key=lambda x: x.cgpa, reverse=True)

# Test the function
class Student:
    def __init__(self, name, roll_number, cgpa):
        self.name = name
        self.roll_number = roll_number
        self.cgpa = cgpa

# Create a list of student objects
students = [
    Student("John Doe", "A123", 3.8),
    Student("Jane Smith", "B456", 3.9),
    Student("Mark Johnson", "C789", 3.5),
    Student("Anna Williams", "D012", 4.0),
]

# Sort the list based on CGPA
sort_students(students)

# Printing the sorted list
for student in students:
    print(f"Name: {student.name}, Roll Number: {student.roll_number}, CGPA: {student.cgpa}")