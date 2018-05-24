import pandas as pd
import numpy as nm
df=pd.DataFrame({'X': [7, 2, 0, 3, 4, 2, 5, 0, 3, 4]})
df['Y']=list((list(df['X'])[i:-1]+[0]).index(0) for i in range(len(df['X'])))
print (df)
