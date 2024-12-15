class Course:
    def __init__(self, course_name, instructor):
        self.course_name = course_name
        self.instructor = instructor

    def get_location(self):
        raise NotImplementedError("Subclasses must implement get_location.")

class OnlineCourse(Course):
    def get_location(self):
        return "www.onlinecourse.com"

class OfflineCourse(Course):
    def get_location(self):
        return "123 College Street"

# Example usage
online_course = OnlineCourse("Python", "John Doe")
offline_course = OfflineCourse("Data Science", "Jane Smith")

print(f"Online course location: {online_course.get_location()}")
print(f"Offline course location: {offline_course.get_location()}")
