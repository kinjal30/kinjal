import matplotlib.pyplot as plt
from numpy import *
import numpy as np
import pandas as pd
import math
fig,ax=plt.subplots()
tips=pd.read_csv("tips.csv")
ax.violinplot(tips["total_bill"],vert=False)
plt.show()
plt.scatter(tips["total_bill"],tips["tip"])
plt.show()
plt.plot(tips["day"],tips["time"])
plt.show()
tips.head(10)
tips['day'].unique()
tips.nunique()
fig1 = plt.figure()
ax1 = fig1.add_subplot(111)
for i in range(1,15):
    ax1.plot(np.array([1,5])*i,label=i)
t = linspace(0,2*math.pi,400)
a = sin(t)
b = cos(t)
c = a + b
plt.plot(t, a, t, b, t, c)
plt.show()
