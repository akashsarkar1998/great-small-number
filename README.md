You can find several ways to find the greater number or smaller number from a given list or the list  which user made.

### ```1. Find greatest number in a list using function:```
```python
def find_largest(numbers):
    max_num = max(numbers)
    return max_num

my_list = []
n= int(input("Enter how many number you want in list: "))
if n>1:
    for i in range(0, n):
        i= int(input())
        my_list.append(i)
    print(my_list)
    result = find_largest(my_list)
    print("the greatest number:", result)
    
else:
    print("List must have at least two elements!")
```

### ```2. Find second greatest number in a list:```
```python
def find_second_largest(numbers):
    max_num = max(numbers)  #used max function to find greatest number
    
    # Remove the maximum number from the list
    numbers.remove(max_num)  #We remove this maximum number from the list using the remove() method.
    
    second_max_num = max(numbers)
    return second_max_num
my_list = []
n= int(input("Enter how many number you want in list: "))
if n>1:
    for i in range(0, n):
        i= int(input())
        my_list.append(i)
    print(my_list)
    result = find_second_largest(my_list)
    print("Second greatest number:", result)
else:
    print("List must have at least two elements!")
```

### ```3. Find second greatest number in a list using sort() method:```
```python
my_list = []
n= int(input("Enter how many number you want in list: "))
if n>1:
    for i in range(0, n):
        i= int(input())
        my_list.append(i)
    print(my_list)
    my_list.sort()
```

### ```4. Find greatest number in a list using sort() method:```
```python
my_list = []
n= int(input("Enter how many number you want in list: "))
if n>1:
    for i in range(0, n):
        i= int(input())
        my_list.append(i)
    print(my_list)
    my_list.sort()
    print(my_list)
    print(f"The Greatest number of the list {my_list} is: ", my_list[-1])
else:
    print("List must have atleast two numbers!")
    print(my_list)
    print(f"The Second greatest number of the list {my_list} is: ", my_list[-2])
else:
    print("List must have atleast two numbers!")
```

### ```5. Find Max or Min number from a list:```
```python
list= [32, 45, 34, 65, 9]
max_num = max(list)
min_num= min(list)
print(max_num)
print(min_num)
```

### ```6. find greatest number!```
```python
list=[]   #ekta empty list banalam! jekhane values store korbo!
n=int(input("How many numbers you want to put: "))  #n er modhe ami set korchi je koto gulo number ani nebo!
for i in range(0, n):   #ebar n ke ami 0 theke iterate korabo!
    i=int(input())   # prottek ta line e ami input nebo. ei prottek ta line holo i,
    list.append(i)   # ekhane prottek line e ami je input nilam, sei i gulo ke ami list e append korchi.
print(list) 
big_num= list[0]
for i in list:
    if i>big_num:
        big_num= i
print(big_num)
```

### ```7. Write a program that repeatedly prompts a user for integer numbers until the user enters 'done'. Once 'done' is entered, print out the largest and smallest of the numbers. If the user enters anything other than a valid number catch it with a try/except and put out an appropriate message and ignore the number. Enter 7, 2, bob, 10, and 4 and match the output below.```
```python
largest = None
smallest = None
while True:
    user_input = (input("Enter a number: "))
    if user_input == "done":
        break
    #print(user_input)
    try:
        num=int(user_input)
        if largest is None or num> largest:
            largest=num
        if smallest is None or num<smallest:
            smallest=num
    except:
        print("Invalid input")
if largest is not None and smallest is not None:
    print("Maximum is", largest)
    print("Minimum is", smallest)
else:
    print("No valid numbers entered.")
```

### ```8. To find Min Value using Accumulation!```
```python
list=[5,3,4,9,6,1,0.5]
min= list[0]
for i in list:
    if i<min:
        min = i
print(i)
```
