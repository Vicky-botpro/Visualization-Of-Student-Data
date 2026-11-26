import sqlite3
import matplotlib.pyplot as plt

connection = sqlite3.connect("SchoolDB.db")
cursor = connection.cursor()

cursor.execute("""
CREATE TABLE IF NOT EXISTS students (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    name TEXT NOT NULL,
    age INTEGER,
    student_class TEXT,
    maths INTEGER,
    science INTEGER,
    maths_result TEXT,
    science_result TEXT
)
""")

connection.commit()


def add_student():

    print("\nADD STUDENT")

    name = input("Enter student name: ")
    age = int(input("Enter age: "))
    student_class = input("Enter class: ")

    maths = int(input("Enter Maths marks: "))
    science = int(input("Enter Science marks: "))

    maths_result = "Passed" if maths >= 40 else "Failed"
    science_result = "Passed" if science >= 40 else "Failed"

    cursor.execute("""
    INSERT INTO students
    (name, age, student_class, maths, science, maths_result, science_result)
    VALUES (?, ?, ?, ?, ?, ?, ?)
    """, (name, age, student_class, maths, science,
          maths_result, science_result))

    connection.commit()

    print("\nStudent added successfully!")


def delete_student():

    print("\nDELETE STUDENT")

    student_id = int(input("Enter student ID: "))

    cursor.execute("""
    DELETE FROM students
    WHERE id = ?
    """, (student_id,))

    connection.commit()

    if cursor.rowcount > 0:
        print("Student deleted successfully!")
    else:
        print("Student not found.")


def view_students():

    print("\nVIEW STUDENTS")

    cursor.execute("""
    SELECT id, name, age, student_class,
           maths, maths_result, science, science_result
    FROM students
    ORDER BY id
    """)

    students = cursor.fetchall()

    if not students:
        print("No students found.")
        return

    print("\n+----+----------------------+-----+-------+-------+----------+---------+----------+")
    print("| ID | Name                 | Age | Class | Maths | Result   | Science | Result   |")
    print("+----+----------------------+-----+-------+-------+----------+---------+----------+")

    for student in students:
        print(
            f"| {student[0]:<2} "
            f"| {student[1]:<20} "
            f"| {student[2]:<3} "
            f"| {student[3]:<5} "
            f"| {student[4]:<5} "
            f"| {student[5]:<8} "
            f"| {student[6]:<7} "
            f"| {student[7]:<8} |"
        )

    print("+----+----------------------+-----+-------+-------+----------+---------+----------+")

def Graph():
# Existing data
    hours = [1, 2, 3, 4, 5, 6, 7]
    marks = [45, 50, 58, 65, 72, 80, 98]

    # Simple prediction for 4.5 hours
    # 4 hours = 65 marks
    # 5 hours = 72 marks
    predict_hour = 4.5
    predict_marks = (65 + 72) / 2

    plt.figure(figsize=(12, 5))

    # Graph 1: Data Visualization
    plt.subplot(1, 2, 1)

    plt.plot(hours, marks, marker='o',
            color='blue')

    plt.title("Study Hours vs Marks")
    plt.xlabel("Study Hours")
    plt.ylabel("Marks")
    plt.grid(True)

    # Graph 2: Data Prediction
    plt.subplot(1, 2, 2)

    plt.plot(hours, marks, marker='o',
            color='green', label='Actual Data')

    plt.scatter(predict_hour, predict_marks,
                color='red', s=120,
                label='Predicted Marks')

    plt.annotate("Predicted: 68.5",
                (predict_hour, predict_marks),
                xytext=(5, 52),
                arrowprops=dict(arrowstyle='->'))

    plt.title("Marks Prediction")
    plt.xlabel("Study Hours")
    plt.ylabel("Marks")
    plt.legend()
    plt.grid(True)

    plt.tight_layout()
    plt.show()

    print("Predicted Marks:", predict_marks)


while True:

    print("\n========== SCHOOL DATABASE ==========")
    print("1. Add Student")
    print("2. Delete Student")
    print("3. View Students")
    print("4. View Student Graph")
    print("5. Exit The Database")

    choice = input("\nChoose an option: ")

    if choice == "1":
        add_student()

    elif choice == "2":
        delete_student()

    elif choice == "3":
        view_students()

    elif choice == "4":
        Graph()
   
    elif choice == "5":
        break
    
    else:
        print("Invalid option. Try again.")


connection.close()
print("Database closed.")
