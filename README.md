# Students-Marks-using-Numpy

 import numpy as np
 
 marks = np.array([67, 78, 98, 89, 79, 67, 79, 95, 68, 97, 93, 59, 81, 79, 99])
 mean = np.mean(marks)
 top = np.max(marks)
 avg = marks[marks < 40]
 
 grade = np.percentile(marks, 75)
 above_avg = marks[marks > mean]
 passed = marks[marks >= 40]
 
 print("Mean Marks:", mean)
 print("Top marks:", top)
 print("Average Student:", avg)
 print("Top 25% cutoff:", grade)
 print("Passed students:", len(passed))
 print("Above average scores:", above_avg)
 print("Lowest marks:", np.min(marks))
 print("Sorted:", np.sort(marks))
