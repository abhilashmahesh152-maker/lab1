
# Student Grade Calculator

print("===== STUDENT GRADE CALCULATOR =====")

name = input("Enter student name: ")

marks = []

for i in range(1, 6):
    mark = float(input(f"Enter marks in subject {i}: "))
    marks.append(mark)

total = sum(marks)
average = total / 5

print("\n===== RESULT =====")
print("Student Name:", name)
print("Total Marks:", total)
print("Average:", average)

if average >= 90:
    grade = "A+"
elif average >= 80:
    grade = "A"
elif average >= 70:
    grade = "B"
elif average >= 60:
    grade = "C"
elif average >= 40:
    grade = "D"
else:
    grade = "Fail"

print("Grade:", grade)
