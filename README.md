# Students-Marks-using-Numpy

 import numpy as np
 import pandas as pd
import matplotlib.pyplot as plt
 
 marks = np.array([67, 78, 98, 89, 79, 67, 79, 95, 68, 97, 93, 59, 81, 79, 99])

 
df = pd.DataFrame({
    "student":[f"S{i+1}" for i in range(len(marks))],
    "marks": marks
})

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


plt.figure()
plt.plot(df["student"], df["marks"], marker="o")
plt.title("Students Marks Trends")
plt.xlabel("students")
plt.ylabel("Marks")
plt.xticks(rotation=45)
plt.show()
