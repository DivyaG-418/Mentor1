# Q1

import pandas as pd

arr = [3,5,7,8,6,5]

arr1 = pd.Series(arr)

print(arr1)


# Q4


arr = pd.Series([3,5,7,8,6,5])

arr1 = pd.Series([4,6,8,7,5,4])

print(arr == arr1)

print(arr > arr1)

print(arr < arr1)


# Q5

dict = {'a': 100, 'b': 200, 'c':300, 'd':400, 'e':800}

arr = pd.Series(dict)

print(arr)


# Q6

import numpy as np

arr = np.array([3,5,5,8,0,7])

arr1 = pd.Series(arr)

print(arr1)


# Q7

arr = pd.Series([3,5,'abcd',7,8,6,5])

arr1 = pd.to_numeric(arr, errors = 'coerce')

print(arr1)

# Q8

arr = {'col1': [1, 2, 3, 4, 7, 11], 'col2': [4, 5, 6, 9, 5, 0], 'col3': [7, 5, 8, 12, 1,11]}

print(pd.Series(df['col1'])


# Q9

arr = pd.Series([3,5,'abcd',7,8,6,5])

arr1 = np.array(arr.values.tolist())

print(arr1)

# Q10

arr = pd.Series([3,5,'abcd',7,8,6,5])

arr1 = arr.sort_values(ascending = True)

print(arr1)

