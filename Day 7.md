# Q1


class Bank_Acc:

    def __init__(self):
    
        self.bal = 0
        

    def deposit(self):
    
        amt = float(input("Enter amount to be deposited"))
        
        self.bal = self.bal+amt
        
        print("Amount deposited",amt)
        

    def withdraw(self):
    
        amt = float(input("Enter amount to be withdrawn"))
        
        if self.bal>= amt:
        
            self.bal-=amt
            
            print("You withdrew",amt)
            
        else:
        
            print("Insufficient balance")
            
            
s= Bank_Acc()

s.deposit()

s.withdraw()



# Q2


class Circle():

    def __init__(self,r):
    
        self.radius = r
        

    def area(self):
    
        return self.radius**2*3.14
        

    def perimeter(self):
    
        return 2*self.radius*3.14
        


New = Circle(5)

print(New.area())

print(New.perimeter())



# Q3


class Shape():

    def __init__(self):
    
        pass
        
    
    def area(self):
    
        return 0
        

class Square(Shape):

        def __init__(self,l):
        
            self.length = l
            

        def area(self):
        
            return self.length**2
            
            Shape.__init__(self)
            

b = Square(2)

print(Square.area())



# Q4


import sys

class ref():

    def reference(self):
    
        print("A")
        

A1 = ref()

a2 = A1

print(sys.getrefcount(A1))


# Q5


class Sal():

    def __init__(self,pay,bonus):
    
        self.pay = pay
        
        self.bonus = bonus
        

    def annual_sal(self):
    
        return (self.pay*12)+self.bonus
        

class emp():

    def __init__(self,name,age,pay,bonus):
    
        self.name = name
        
        self.age = age
        
        self.obj_sal = Sal(pay,bonus)
        

    def total_sal(self):
    
        return self.obj_sal.annual_sal()
        

employee = emp('max',25,20000,5000)

print(employee.total_sal())




            
            

