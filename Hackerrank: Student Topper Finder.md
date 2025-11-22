# # 🔢 Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.

---
## 💻 PROGRAM:
```
input_str = input()
marks_dict = eval(input_str)

total_marks_dict = {}

for name, marks in marks_dict.items():
    total = sum(marks)
    total_marks_dict[name] = total

print(total_marks_dict)

topper = max(total_marks_dict, key=total_marks_dict.get)
top_score = total_marks_dict[topper]

print("Topper is: ",  topper, "with marks = ",  top_score)
```

## OUTPUT
<img width="1127" height="191" alt="image" src="https://github.com/user-attachments/assets/b744b869-c571-4b8a-b9d4-36834ca2a09b" />

print("Topper is: ",  topper, "with marks = ",  top_score)
## RESULT
Thus, the output is verified successfully
