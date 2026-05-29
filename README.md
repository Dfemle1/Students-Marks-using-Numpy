# Students-Marks-using-Numpy

 import numpy as np
>>> marks = np.array([67, 78, 98, 89, 79, 67, 79, 95, 68, 97, 93, 59, 81, 79, 99])
>>> mean = np.mean(marks)
>>> top = np.max(marks)
>>> avg = marks[marks < 40]
>>> grade = np.percentile(marks, 75)
print("Mean Marks:", mean)
Mean Marks: 81.86666666666666
>>> print("Top marks:", top)
Top marks: 99
>>> print("Average Student:", avg)
Average Student: []
>>> print("Top 25% cutoff:", grade)
Top 25% cutoff: 94.0
>>>
>>> passed = marks[marks >= 40]
>>> print("Passed students:", len(passed))
Passed students: 15
>>> above_avg = marks[marks > mean]
>>> print("Above average scores:", above_avg)
Above average scores: [98 89 95 97 93 99]
>>> print("Lowest marks:", np.min(marks))
Lowest marks: 59
>>> print("Sorted:", np.sort(marks))
Sorted: [59 67 67 68 78 79 79 79 81 89 93 95 97 98 99]
