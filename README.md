
# 19CS301-Module10
- **Name:** Nevil Joe Ferdin P
- **Registration Number:** 212222050041
## ExNo: 10.1 Stack
### Aim: 
To write a python program to get the integer values from the user and push only the odd number into the stack and later pop the last 2 elements
### Algorithm:

**STEP 1:** Start.

**STEP 2:** Create an empty list `stack` to act as a stack.

**STEP 3:** Take input `n` from the user (number of elements).

**STEP 4:** Repeat steps 5 to 7 for `i` from 0 to `n-1`.

**STEP 5:** Take an integer input `a`.

**STEP 6:** Check if `a` is odd (i.e., `a % 2 != 0`).

**STEP 7:** If odd, append `a` to the `stack`.

**STEP 8:** Print the current `stack`.

**STEP 9:** Remove the top 2 elements from the stack using `pop()`.

**STEP 10:** Print the modified stack.

**STEP 11:** Stop.

### Program:
```python
stack=[]
n=int(input())
for i in range(n):
    a=int(input())
    if a%2!=0:
        stack.append(a)
print(stack)
for i in range(2):
    stack.pop()
print(stack)

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/406fdf71-4069-4125-b3f5-396c7750ca3d)

### Result: 
Thus, the given program is implemented and executed successfully .

## ExNo: 10.2 Implementation of Stack
### Aim: 
To write a python program to check whether the given  string is palindrome
### Algorithm:

**STEP 1:** Start.

**STEP 2:** Take a string input `a` from the user.

**STEP 3:** Reverse the string using slicing `a[::-1]`.

**STEP 4:** Compare the original string `a` with its reversed version.

**STEP 5:** If both are equal, print `"Yes"` (the string is a palindrome).

**STEP 6:** Otherwise, print `"No"` (the string is not a palindrome).

**STEP 7:** Stop.

### Program:
```python
a= input()
if a==a[::-1]:
    print("Yes")
else:
    print("No")

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/d2ba47e7-c4f7-4fc8-ae4a-dffcc5ab0fd6)

### Result: 
Thus, the given program is implemented and executed successfully .

## ExNo: 10.3 Queue
### Aim: 
To develop a python program to add only the even unique numbers using appendleft() from n given numbers
### Algorithm:

**STEP 1:** Start.

**STEP 2:** Import `deque` from the `collections` module.

**STEP 3:** Define a function `add_even(n, stack)`:
  - Create an empty deque `d`.
  - Create an empty set `unique` to store seen even numbers.
  - Loop through each element `i` in the list `stack`.
    - If `i` is even and not already in `unique`:
      - Add `i` to the left of deque `d` using `appendleft()`.
      - Add `i` to the set `unique`.

**STEP 4:** Take an integer input `n` from the user (number of elements).

**STEP 5:** Take `n` integer inputs from the user and store them in a list called `stack`.

**STEP 6:** Call the function `add_even(n, stack)`.

**STEP 7:** Inside the function, print the final deque.

**STEP 8:** Stop.

### Program:
```pyhton
from collections import deque
def add_even(n,stack):
    d=deque()
    unique=set()
    for i in stack:
        if i%2==0 and i not in unique:
            d.appendleft(i)
            unique.add(i)
    print(f"deque({list(d)})")
n= int(input())
stack=[int(input()) for _ in range(n)]
add_even(n,stack)

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/0a43b200-15b2-4cb8-be71-d999fbb138c2)

### Result:
Thus, the given program is implemented and executed successfully .

# ExNo: 10.4 Types of Queue
### Aim:
To develop a python program to get the 4 integer values from user and display the values  using multiprocessing library
### Algorithm:

**STEP 1:** Start.

**STEP 2:** Create an empty list `l`.

**STEP 3:** Repeat the following steps 4 times:
  - Take an integer input from the user.
  - Append the input to the list `l`.

**STEP 4:** Traverse the list `l` using a loop:
  - Print each element of the list.

**STEP 5:** Stop.

### Program:
```python
l=[]
for i in range(4):
    l.append(int(input()))
for i in l:
    print(i)

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/c0ebdf92-9610-454e-9ab6-65f6c7dd8b5f)

### Result: 
Thus, the given program is implemented and executed successfully .
