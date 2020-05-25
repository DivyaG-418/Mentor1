# Q1.

def lrgst(a,b,c):

    if (a<b) or (a<c):
    
        if (b<c):
        
            print(c,"is the greatest")
            
        else:
        
            print(b,"is the greatest")
            
    else:
    
        print(a, "is the greatest")
        

lrgst(9,3,19)


# Q2.

def local():

    x = 10
    
    y = 20
    
    z = 30
    
print("No. of local variables", local.__code__.co_nlocals)


# Q3.

def recurs(n):

    if n<=0:
    
      return n
      
    return n + recurs(n-1)
    

n = 10

print(recurs(n))


# Q4.

def showStudent(name, student_id = 1, college_name = 'Vita'):

    print(name, student_id, college_name)
    

showStudent('Divya')


# Q5.


def lst(l):

    lst2 = set(l)
    
    return lst2
    

    
l =  [11,22,22,33,33,33,44,55,55,66]

div = lst(l)

print(div)



# Q6

def frst_lst(dgt):

    for i in range(0,len(dgt)):
    
        sum = int(dgt[0]) + int(dgt[-1])
        
        return sum
        

print(frst_lst(input("Enter number")))
    
    
    











    
