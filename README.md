🎓 CGPA Calculator (C++)

A console-based C++ application to calculate semester-wise GPA and overall CGPA using a weighted average approach.
Built with clean logic, modular structure, and academic grading standards in mind.

✨ Features
> Multi-semester CGPA calculation
> Weighted average formula
> Grade-to-grade-point conversion
> Scalable & modular C++ code
> User-friendly console interaction

🛠️ Tech Stack
Language: C++
Compiler: GCC / MinGW
IDE: VS Code / Code::Blocks
Platform: Windows / Linux

Grade	Points
O	               10
A+	              9
A	                8
B+	              7
B	                6
C	                5
F	                0
ℹ️ Grade mapping can be modified easily in the source code.
📌 UML Class Diagram

The following UML diagram represents the logical structure of the CGPA Calculator system.
It shows how student data, courses, and CGPA calculation logic are organized.

+------------------+
|     Student      |
+------------------+
| - semesters      |
+------------------+
| + inputData()    |
| + calculateCGPA()|
+------------------+
          |
          |
          v
+------------------+
|    Semester      |
+------------------+
| - courses        |
| - semesterGPA    |
+------------------+
| + inputCourses() |
| + calculateGPA() |
+------------------+
          |
          |
          v
+------------------+
|     Course       |
+------------------+
| - grade          |
| - credits        |
| - gradePoint     |
+------------------+
| + convertGrade() |
+------------------+

+---------------------------+
|     CGPACalculator        |
+---------------------------+
| + calculateWeightedAvg()  |
+---------------------------+


📌 UML Activity Diagram (CGPA Calculation Flow)
(Start)
   |
   v
[Display Menu]
   |
   v
[Enter Semester Count]
   |
   v
[For each Semester]
   |
   v
[Enter Courses, Grades, Credits]
   |
   v
[Convert Grade to Grade Point]
   |
   v
[Calculate Semester GPA]
   |
   v
[Add to Total Credits & Points]
   |
   v
[Calculate Final CGPA]
   |
   v
(Display Result)
   |
  (End)
  

📌 UML Use Case Diagram
       +--------+
       |  User  |
       +--------+
            |
            |
   --------------------
   |       |          |
   v       v          v
[Enter Data] [View GPA] [View CGPA]
