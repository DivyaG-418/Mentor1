# Q1


dic = {'Divya' :27, 'Nikhil' : 29, 'Neha' : 25, 'Rutuja': 15, 'Pushti': 14}

new = dict([(value, key)for key, value in dic.items()])

print("keys: values")

for i in new:

    print( i , " :" , new[i],end='')
    


# Q2.
'''
A = [35, 67, 86, 25, 86, 56]

for i in range(len(A)):

    min_pos = i
    
    for j in range(i+1, len(A)):
    
        if A[min_pos] > A[j]:
        
            min_pos = j
            
    A[i], A[min_pos] = A[min_pos], A[i]


for i in range(len(A)):

    print("%d" %A[i])
    


# Q3


def sort(arr):

    for i in range(1, len(arr)):
    
        key = arr[i]
        
        j = i-1
        
        while j>= 0 and key< arr[j]:
        
            arr[j+1] = arr[j]
            
            j -= 1
            
        arr[j+1] = key
        


arr = [43, 56, 12, 98, 57, 22, 44]

sort(arr)

for i in range(len(arr)):

    print("%d" %arr[i])
    


# Q4


list1 = ['a', 'b', ['c', ['d', 'e', ['f', 'g'], 'k'], 'l'], 'm', 'n'] 

list1[-3][-2][-2].extend(['h', 'i', 'j'])

print(list1)


# Q5

sampleDict = { 

   "class":{ 
   
      "student":{ 
      
         "name":"Mike",
         
         "marks":{ 
         
            "physics":70,
            
            "history":80
            
         }
         
      }
      
   }
   
}


print(sampleDict['class']['student']['marks']['history'])


