# 19CS301Module-9
### EX: 9.1                                            MATRIX OPERATIONS
### Aim:
To Write a Python Program to subtract two matrices by reading the matrix from the user.
### Algorithm:

STEP 1: Start.

STEP 2: Create a variable r and c for rows and columns of the matrix.

STEP 3: Get the value of r and c from user.

STEP 4: Define a function to create a matrix.

STEP 5 : Define another function to subtract the matrices.

STEP 6: Print the result.

STEP 7 : Stop.
### Program:
```
def create_matrix(n,m):
         M = []
         for i in range(n):
                   row = []
                   for j in range(m):
                      x = int(input())
                       row.append(x)
           M.append(row)
         return M
r,c = input().split()
A = create_matrix(int(r),int(c))
B = create_matrix(int(r),int(c))
C = []
for i in range(int(r)):
         R = []
 

        for j in range(int(c)):
                item = A[i][j]-B[i][j]
   R.append(item)
C.append(R)
print(A)
print(B)
print(C)
```
### Output:
![image](https://github.com/user-attachments/assets/b1125b13-d26e-4404-acce-7dd2c1d2011c)

### Result: Thus, the given program is implemented and executed successfully .

### EX: 9.2 LIST COMPREHENSION
### Aim:
To Write a Python class program to generate all even numbers between 200 and 300 and store in a list using list comprehension.
### Algorithm:
STEP 1: Start.

STEP 2: Create a class.

STEP 3: Create variable a,b, and c for upper limit,lower limit and condition.

STEP 4: Intialise the values in the class.

STEP 5 : Define a method and using list comprehension calculate the result.

STEP 6: Print the result.

STEP 7 : Stop.

### Program:
```
class program:

      def  __init__(self,a,b,c):
                self.a=a
                self.b=b
                self.c=c
        def display(self):
               even = [i for i in range(self.a,self.c+1,self.b)]
               print(even)
a = int(input())
b = int(input())
c = int(input())

obj = program(a,b,c)
obj.display()
```
### Output:
 ![image](https://github.com/user-attachments/assets/a9707d46-2d47-4472-a6b3-b407a6f6ef71)

### Result: Thus, the given program is implemented and executed successfully .

### EX: 9.3 ADVANCED LIST PROCESSING
### Aim:
To Write a Python program to add two matrix using list Comprehension.

### Algorithm:

STEP 1: Start.

STEP 2: Create a variable r and c for rows and columns. 

STEP 3: Get the value of r and c from user.

STEP 4: Define a function to create the matrix.

STEP 5 : Using list comprehension add the two matrix.

STEP 6: Print the result.

STEP 7 : Stop.

### Program:
```
def create_matrix(n,m):
    M=[]
    for i in range(n):
        row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
    return M 
    
r,c=input().split()
r=int(r)
c=int(c)
A=create_matrix(r,c)
B=create_matrix(r,c)
print(A)
print(B)
T = [[A[i][j]+B[i][j] for j in range(len(A[0]))]for i in range(len(A))]
print(T)
```
### Output:
![image](https://github.com/gokulkrishnan2005/19CS301Module-9/blob/main/module%209-1.png)

### Result: Thus, the given program is implemented and executed successfully .
 


### EX: 9.4       TOEPLITZ MATRIX
### Aim:
To Write a Python Program to check whether the given matrix is Toeplitz Matrix.


### Algorithm:
STEP 1: Start.

STEP 2: Create a variable r and c for rows and columns.

STEP 3: Get the value of r and c from user.

STEP 4: Define a function to create the matrix.

STEP 5 : Using the formula check for TOEPLITZ MATRIX .

STEP 6: Print the result.

STEP 7 : Stop.


### Program:
```
def create_matrix(n,m):
        M=[]
        for i in range(n):
                row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
      return M
def print_matrix(M):
    for i in range(len(M)):
         for j in range(len(M[0])):
               print(M[i][j], end=' ')
     print()
def isThoeplitz(M):
#Type your code here
for i in range(len(M)):
      for j in range(len(M[0])):
             if i>0 and j>0 and M[i][j]!=M[i-1][j-1]:
                return False
       return True
n,m = input().split()
A = create_matrix(int(n),int(m))
print("A=",A)
if isThoeplitz(A):
      print(A,"is a Toeplitz Matrix")
 else:
       print(A,"is not a Toeplitz Matrix") print_matrix(A)
```
### Output:

![image](https://github.com/user-attachments/assets/0fb8f81b-ab07-4b3e-b273-035a0f38566d)

### Result: Thus, the given program is implemented and executed successfully.


 ### EX: 9.5 SEB- LIST COMPREHENSION
### Aim:
To Write a Python program to find the cube of all elements in a list using list comprehension.
### Algorithm:
Start

Read an integer n (number of elements).

Initialize an empty list l.

Repeat steps 5–6, n times:

Read a floating-point number x.

Append x to the list l.

Create a new list sq_l:

For each element item in list l, compute item ** 3 and store it in sq_l.

Print the original list l.

Print the cubed list sq_l.

End



### Program:
```
n=int(input())
l=[]
for i in range(n):
    x=float(input())
    l.append(x)
sq_l=[item**3 for item in l]
print(l)
print(sq_l)
```
### Output:
 ![image](https://github.com/gokulkrishnan2005/19CS301Module-9/blob/main/m9%205th.png)

### Result: Thus, the given program is implemented and executed successfully .

