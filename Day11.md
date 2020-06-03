# Q1

import numpy as np

a = np.arange(1,13).reshape(3,4)

print(a)
for x in np.nditer(a):

    print(x)
    

# Q2


v = np.arange(5,51,5)

print(v[1:-1])


# Q3

x = np.arange(0,21)

x[(x>=9) & (x<=15)]*= -1

print(x)


# Q4

abc = np.random.randint(0,11,5)

print(abc)


# Q5


v1 = ([3,4,5,7,8,6,3,2])

v2 = ([7,5,4,3,9,7,5,4])

for i in range (len(v1)):

    for j in range (len(v2)):
    
        if i == j:
        
            print(v1[i]*v2[j])
            


# Q6

a = np.arange(10,22).reshape(3,4)

print(a)


# Q7

a = np.arange(10,22).reshape(3,4)

print(a.shape)


# Q8

a = np.identity(3)

print(a)


# Q9

s = np.ones((10,10))

s[1:-1, 1:-1] = 0

print(s)


# Q10

d = np.diag([1,2,3,4,5])

print(d)


# Q11

arr = np.zeros((4,4))

arr[::2, 1::2] = 1

arr[1::2, ::2] = 1

print(arr)


# Q12

z = np.random.random((3,3,3))

print(z)


# Q13

r = np.array([[3,4], [5,6]])

print(np.sum(r))

print(np.sum(r,axis=0))

print(np.sum(r,axis=1))



# Q14

y = np.array([7,8])

z = np.array([4,2])

print(np.dot(y,z))



# Q15

a = np.array([[1,2,3], [4,5,6], [7,8,9], [10,11,12]])

b = np.array([1,1,0])

res = np.empty_like(a)

for i in range(4):

    res[i, :] = a[i, :] +b
    
print(res)

