class Mentor:
    def __init__(self, n, c):
        self.name = n
        self.courses = c

mentor_1 = Mentor('Иванов Петр', 'Python')
mentor_2 = Mentor('Давыдов Олег', 'Java')
mentor_3 = Mentor('Семенов Алексей', 'Data')

print(mentor_1.name, mentor_1.courses)
print(mentor_2.name, mentor_2.courses)
print(mentor_3.name, mentor_3.courses)

class Lecturer(Mentor):
    def __init__(self, n, c, l):
        self.name = n
        self.courses = c
        self.lecturer= l

lecturer_1 = Lecturer('Иванов Петр,', 'Курс: Python,', 'лектор')

print(lecturer_1.name, lecturer_1.courses, lecturer_1.lecturer)

class Reviewer(Mentor):
    def __init__(self, n, c, r):
        self.name = n
        self.courses = c
        self.reviewer = r

reviewer_1 = Reviewer('Давыдов Олег,', 'курс: Java,', 'эксперт, проверяющий задания')
reviewer_2 = Reviewer('Семенов Алексей,', 'курс: Data', 'эксперт, проверяющий задания')

print(reviewer_1.name, reviewer_1.courses, reviewer_1.reviewer)
print(reviewer_2.name, reviewer_2.courses, reviewer_2.reviewer)