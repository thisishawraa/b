class Student:
    def __init__(self, name, grades):
        self.name = name
        self.grades = grades

    def check_status(self):
        return "Pass" if self.grades >= 50 else "Fail"

# إنشاء كائنين وطباعة النتائج
student1 = Student("Ali", 85)
student2 = Student("Sara", 45)
print(student1.name, student1.check_status())
print(student2.name, student2.check_status())
