# Q1.

def bubble(arr):

    n = len(arr)
    
    for i in range(n):
    
        for j in range(0, n-i-1):
        
            if arr[j] > arr[j+1]:
            
                arr[j], arr[j+1] = arr[j+1], arr[j]
                


arr = [45, 23, 87, 12, 76, 98, 55]

bubble(arr)

print("Sorted array is")

for i in range(len(arr)):

    print("%d" %arr[i])



# Q2.


def linear(arr, n):

    for i in range(len(arr)):
    
        if arr[i] == n:
        
            print(i)
            

arr = [45, 23, 87, 12, 76, 98, 55]

linear(arr, 12)



# Q3.


def bin_search(list1, item):

    first= 0
    
    last=len(list1)-1
    
    found=False
    

    while(first<=last and not found):
    
        mid= (first+last)//2
        

        if list1[mid]==item:
        
            found = True
            

        else:
        
            if item < list1[mid]:
            
                last=mid - 1
                
            else:
            
                first=mid + 1
                
    return found
    

num=bin_search([11,22,33,44,55,66],66)

print(num)


num=bin_search([11,22,33,44,55,66],77)

print(num)

            
# Q4.


List1 = ["M","na","i","lak"]

List2 = ["y","me","s","han"]

result = [i+j for i,j in zip(List1, List2)]

print(str(result))



# Q5.

def dictionary(dict, n):

    if n in dict:
    
        print("Value=", dict[n], end=" ")
        
        print("Present")
        
    else:
    
        print("Not present")
        


dict = {"John":47,"Peter":64,"Mahi":37,"Maria":76}

n = "Peter"

dictionary(dict, n)



    

