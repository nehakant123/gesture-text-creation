# gesture-text-creation
Assigment 1
Question 1
# Take value of n (dtype = float) as an input from user and print it 
n = 3.4
Answer 
value=float(input("Enter value of n:"))
print(value)

Question 2
# Check if the input value is integer or not
# If not integer then keep on taking the values from user until the input value is integer
# And check whether the integral input value is even or odd

while         :
  if    :
    

  else        :
    
    
    
    
if       :
  if      :
    print(f"n={n} is even")
  else    :
    print(f"n={n} is odd")
n=3.4 is not an integer
n=4.56 is not an integer
n=5.0 is an Integer
n=5.0 is odd
Answer
i=1
while(i>0):
    value=input()
    if(value.isnumeric()):
        i=-1
        print("n ="+value+" is an integer")
    else:
        i=i+1
        print("n ="+value+" is not integer")
        
if(i==-1):
    if(int((value))%2==0):
        print("n ="+value+" is even")
    else:
         print("n ="+value+"is odd")

Question 3
# Define an array and take its elements as input
import numpy as np

n =
arr = 
Answer
import numpy as np
n=int(input())
arr=np.array([0]*n)
for i in range(0,n):
    a=input()
    arr[i] =a 

print(arr)

#Question 4
# Implement a function on the matrix
# Function should make each row's diagonal element to be maximum in its row irrespective of sign
# Output the matrix and intermediate steps

def diagonallyDominant(arr, verbose=False):
    n = arr.shape[0]
   return arr

print("Original matrix: ")
print(arr)
print("_"*100,"\n")

A = diagonallyDominant(arr, verbose=True)
print("_"*100,"\n")

print("Matrix obtained is: ")
print(A)
Answer 
import numpy as np
def diagonallyDominant(arr,n, verbose=False):
    for i in range(0,n):
        max=0
        i1=0
        j1=0 
        for j in range(0,n):
            if(abs(max)<abs(arr[i][j])):
                max=arr[i][j] 
                i1=i
                j1=j
        arr[i1][j1]=arr[i][i]
        arr[i][i]=max
        print(arr)                 

    return arr

n=int(input())
a=np.array([0]*(n*n))
for i in range(0,(n*n)):
    b=int(input())
    a[i]=b
arr=a.reshape(n,n)
    
print("Original matrix: ")
print(arr)
print("_"*100,"\n")

A = diagonallyDominant(arr,n, verbose=True)
print("_"*100,"\n")

print("Matrix obtained is: ")
print(A)
Question 5
## Check the changed matrix (matrix obatined above) is diagonally dominant or not?
Answer
import numpy as np
def diagonallyDominant(arr,n, verbose=False):
    for i in range(0,n):
        max=0
        i1=0
        j1=0 
        for j in range(0,n):
            if(abs(max)<abs(arr[i][j])):
                max=arr[i][j] 
                i1=i
                j1=j
        arr[i1][j1]=arr[i][i]
        arr[i][i]=max
        print(arr)                 

    return arr

n=int(input())
a=np.array([0]*(n*n))
for i in range(0,(n*n)):
    b=int(input())
    a[i]=b
arr=a.reshape(n,n)
    
print("Original matrix: ")
print(arr)
print("_"*100,"\n")

A = diagonallyDominant(arr,n, verbose=True)
print("_"*100,"\n")

print("Matrix obtained is: ")
print(A)
row_sum=0
cnt=0
sum=0
arr=A
for i in range(0,n):
    max=abs(arr[i][i])
    sum=0
    for j in range(0,n):
     sum=sum+abs(arr[i][j])
    sum=sum-max
    if(max>=sum):
        cnt=cnt+1

if (cnt==n):
  print(f"{A} is diagonally dominant")
  
else :
  print(f"{A} \n is not diagonally dominant")

  Question 5 part 2
  import numpy as np
def diagonallyDominant(arr,n, verbose=False):
    for i in range(0,n):
        max=0
        i1=0
        j1=0 
        for j in range(0,n):
            if(abs(max)<abs(arr[i][j])):
                max=arr[i][j] 
                i1=i
                j1=j
        arr[i1][j1]=arr[i][i]
        arr[i][i]=max
        print(arr)                 

    return arr

n=int(input())
a=np.array([0]*(n*n))
for i in range(0,(n*n)):
    b=int(input())
    a[i]=b
arr=a.reshape(n,n)
    
print("Original matrix: ")
print(arr)
print("_"*100,"\n")

A = diagonallyDominant(arr,n, verbose=True)
print("_"*100,"\n")

print("Matrix obtained is: ")
print(A)
row_sum=0
cnt=0
sum=0
arr=A
for i in range(0,n):
    max=abs(arr[i][i])
    sum=0
    for j in range(0,n):
     sum=sum+abs(arr[i][j])
    sum=sum-max
    if(max>=sum):
        cnt=cnt+1
    else:
       print("Row index =",end=" ")
       print(i)
       print("Elements :",end=" ")
       for g in range(0,n):
          print(arr[i][g],end=" ")

print()
if (cnt==n):
  print(f"{A} is diagonally dominant")
  
else :
  print(f"{A} \n is not diagonally dominant")

 Question 6
Relu function 

from matplotlib import pyplot as plt
import numpy as np
import math
def fun(x_val):
    return(np.maximum(0,x_val))
    
x_val = np.linspace(-100,100, 10000)
ans=fun(x_val)
plt.plot(x_val,ans)
plt.show()

Tanh and sigmoid function

from matplotlib import pyplot as plt
import numpy as np
import math
def fun(x_val):
    return(1/(1+np.exp(-x_val)))

def fun1(x_val):
    return((np.exp(x_val)-np.exp(-x_val))/(np.exp(x_val)+np.exp(-x_val)))

    
x_val = np.linspace(-100,100, 10000)
ans=fun(x_val)
plt.plot(x_val,ans)
ans1=fun1(x_val)
plt.plot(x_val,ans1)
plt.show()

Question 7
Answer
from matplotlib import pyplot as plt
import numpy as np
import math

def fun(x_val):
    return(np.maximum(0,x_val))

def fun2(x_val):
    return(1/(1+np.exp(-x_val)))

def fun1(x_val):
    return((np.exp(x_val)-np.exp(-x_val))/(np.exp(x_val)+np.exp(-x_val)))

n=int(input())
a=np.array([0]*(n*n))
for i in range(0,(n*n)):
    b=int(input())
    a[i]=b
arr=a.reshape(n,n)

x_val=np.array([0]*n)
for i in range(0,n):
    x_val[i]=arr[i][i]
        

ans=fun(x_val)
plt.scatter(x_val,ans,color='blue')
ans1=fun2(x_val)
plt.scatter(x_val,ans1)
ans2=fun1(x_val)
plt.scatter(x_val,ans2)
plt.show()

Question 9
Answer
from matplotlib import pyplot as plt
import numpy as np
import math

def softmax(arr,n):
    k=0.0
    for i in range(0,n):
        k=np.exp(arr[i])+k
  
    for i in range(0,n):
        arr[i]=np.exp(arr[i])/k
    return(arr)               



n=int(input())
a=np.array([0.0]*(n*n))
for i in range(0,(n*n)):
    b=int(input())
    a[i]=b
arr=a.reshape(n,n)

x_val=np.array([0.0]*n)
for i in range(0,n):
    x_val[i]=arr[i][i]

ans=softmax(x_val,n)
print(ans) 

Question 10
Answer
from matplotlib import pyplot as plt
import numpy as np
import math

def softmax(arr,n):
    k=0.0
    for i in range(0,n):
        k=np.exp(arr[i])+k
  
    for i in range(0,n):
        arr[i]=np.exp(arr[i])/k
    return(arr)               



n=int(input())
a=np.array([0.0]*(n*n))
for i in range(0,(n*n)):
    b=int(input())
    a[i]=b
arr=a.reshape(n,n)

x_val=np.array([0.0]*n)
for i in range(0,n):
    x_val[i]=arr[i][i]

l=x_val.copy()
ans=softmax(x_val,n)
print(ans)  

plt.scatter(ans,l,color='blue')
plt.show()

Question 13
Answer
from matplotlib import pyplot as plt
import numpy as np
import math

def softmax(arr,n):
    k=0.0
    for i in range(0,n):
        k=np.exp(arr[i])+k
  
    for i in range(0,n):
        arr[i]=np.exp(arr[i])/k
    return(arr)               



n=int(input())
a=np.array([0.0]*(n*n))
for i in range(0,(n*n)):
    b=int(input())
    a[i]=b
arr=a.reshape(n,n)

x_val=np.array([0.0]*n)
for i in range(0,n):
    x_val[i]=arr[i][i]

l=x_val.copy()
ans=softmax(x_val,n)

max=ans[0]
index=0
for i in range(0,n):
    if(max<ans[i]):
        max=ans[i]
        index=i

for i in range(0,n):
    if(ans[i]!=max):
        print(l[i],end=" ")
        print(" : Not a max element in all diagonal elements")
        print()
print(l[index],end=" ")
print(" :Max element in all diagonal elements")

Softmax function
It is a mathematical function which converts array of numbers into array of probability. It is widely used in ML to convert raw data into probability along with normalisation of the values. for a given data set if for a particular value the set gives highest probability then it means that value affects the given model the most, and we can also remove some data set of least probability as per requirement.we can also determine a threshold probability value above which we can declare the given model as accurate.Here in this case 406 shows the highest probability while -100 shows the least.

Assigment 1 part-2
Question-1
For supervised learning(or classification) 
Supervised learning is basically a teaching and learning method where the machine learns from a given data set and implement the same learning on a new data set.we train machine with a labelled data set and then checks its learning on a new unlabelled data set. 
It can be classified into two types regression and classification 
Regression works on continuous values.
Classification basically means giving answer in true or false for example if a given email is spam or not , or whether it will rain or not.
We keep on testing this model on different test cases and tries to increase its accuracy.

Unsupervised learning(or clustering)
Essentially it means learning on its own. We do not train machine with labelled data and directly implements it on unlabelled data and the machine tries to find similar data by identifying similar patterns , colour and shape and store it as a cluster.
Unsupervised can be used for recommending movies, song, books ,or clothes  as the model observes similarity in pattern and behaviour of various users. 
Unsupervised learning is uncertain as compared to supervised learning because firstly it works on a model to identify similar patterns which makes this work a bit challenging and it does not have a clear objective like it involves identifying similar patterns and then clustering it or reducing  the dimensionality of data set which somewhat affects the accuracy of the model.

Reinforcement learning
It’s a kind of hit and trial method. The models tries every possible path to reach the solution and then chooses the most optimal path for the problem. The  model completely depends not the decision taken by the software without having any previous experience. It is autonomous. 
Tesla uses reinforcement learning where the car learns the control and navigate itself in various tricky situations.

Both supervised and reinforcement learning have their own strengths and weaknesses like supervised learning is more preferred in case of static and less interactive environment where as reinforcement learning is more preferred for dynamically changing data set and more interactive environment. 



Machine learning vs deep learning 
Deep learning is a subset of machine learning. In machine learning we use supervised learning which requires human intervention whereas in deep learning we use unsupervised learning where the computer itself find abstracts similar patterns by passing data through different layers and tells us about the output and can also work on a large data set. Deep learning involves more than 3 layers. Deep learning requires a large amount of data to work on and can produce more accurate results than machine learning.machine learning relies on human input which limits the model ability to work on new data set.
Deep learning has its own disadvantages like it requires a large amount of labelled data to produce more efficient results and those data sets are expensive whereas ML can produce somewhat same result with less data. Deep learning also requires GPUs which more expensive as compared to CPUs. Developing models of linear regression are more preferred in ML as it does the task in a more simple way.
Both have their own strengths and weaknesses so we should choose between the two on the basis of our problem statement. 

Question 2
def palin(num):
  a=num
  rev=0
  while(a>0):
       b=a%10
       rev=rev*10+b
       print(rev)
       a=a//10
  
  if(rev==num):
      return 1
  else:
      return 0
  

num1=int(input())
ans=palin(num1)
if(ans==1):
    print("true")
else:
    print("false")

Question 3
import numpy as np
arr=np.linspace(1,100,10,dtype="int")
print(arr)
print(arr.mean())
print(arr.min())
print(arr.max())

Question 4
import pandas as pd
import matplotlib.pyplot as plt
df=pd.DataFrame({'Name':['A','B','C','D','E','F','G','H','I','J'],
                 'Age':[21,30,29,32,35,21,22,23,25,19],
                 'City':['Lucknow','Bombay','Mussorie','Vanarasi','Kanpur','Lucknow',
                         'Mussorie','Bombay','Lucknow','Lucknow']})
print(df)
df.query('Age<=30',inplace=True)
print(df)
df['Salary']=[50000,60000,70000,50000,50000,60000,70000,60000]
print(df[['City','Salary']])
by_city=df.groupby(['City'])
print(by_city['Age'].mean())
plt.title("Age vs Salary")
plt.scatter(df['Age'],df['Salary'])
plt.show()
plt.title("City vs Age")
plt.bar(df['City'],df['Age'])
plt.show()
plt.title("Mean salary vs City")
plt.pie(by_city['Salary'].mean(),labels=by_city)
plt.show()


