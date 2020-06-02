# Q1.


import numpy as np

a = np.__version__

print(a)

b = np.show_config()

print(b)



# Q2


d = np.array([4,5,7,3j,4,9j,3+4j])

print(np.isreal(d))

print(np.iscomplex(d))

print(np.isscalar(d))



# Q3.


y = ([3,0,5,0,7,8])

print(np.all(y))



# Q4


x = np.array([3,4,6,8,6,0,5,4,0])

print(np.any(x))



# Q5


a = np.array([5,3,1,0,np.nan])

print(np.isnan(a))



# Q6

a = np.array([5,6])

b = np.array([5,9])

print(np.greater(a,b))

print(np.greater_equal(a,b))

print(np.less(a,b))

print(np.less_equal(a,b))



# Q7


a1 = ([45,76,4,78,55,23.5,77.00])

b1 = ([45,76,4,78,55,23.5,77.001])

print(np.equal(a1,b1))

print(np.allclose(a1,b1))


# Q8


s = np.array([6,5,7,8,4,3])

print("%d" %(s.size*s.itemsize))



# Q9


arr = np.zeros(10)

print(arr)

arr = np.ones(10)

print(arr)

arr = np.ones(10)*5

print(arr)



# Q10


z = np.arange(30,71)

print(z)



# Q11


z = np.arange(30,71,2)

print(z)



# Q12


a = np.identity(3)

print(a)


# Q13


num = np.random.normal(0,1)

print(num)


# Q14


num = np.random.normal(0,1,15)

print(num)



# Q15


v = np.arange(15,55)

print(v[1:-1])


