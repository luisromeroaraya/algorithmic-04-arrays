# [Arrays](https://github.com/becodeorg/BXL-Swartz-4-27/blob/master/1.The-Field/7.Algorithmic/04-arrays.adoc)
* Type of challenge: **learning**
* Duration: **60 min**
* Team challenge: **solo**

## Learning objectives
At the end of this challenge you should:
* understand the concept of arrays
* be able to declare arrays
* be able to assign values to an array
* be able to select a value in an array

## The mission
This challenge will have you play around with the concept of [arrays](https://en.wikipedia.org/wiki/Array_data_type), complete the exercises down below after you’ve read the explanations.

Arrays are variables of sort, but their specificity is that they can hold multiple values at the same time. If a variables is a box holding a value, then an array is a table containing multiple box.

In computer science an array **begins at 0**, meaning that the first element is on the index 0. They have specific sub functions to add ```array.add_value``` and remove ```array.remove_value``` data.

Example
```
// This algorithm will output "Arsène Adalric Aelis".
array names = ["Arsène","Adalric","John"]

remove_value(names[2])
add_value("Aelis",$names)

output($names[0] + " " + $names[1] + " " + $names[2])
```

## Exercises

Instructions
* write your algorithm on paper
* detail each and every step
* indicates the types of used variables

*I will be using [Python3](https://repl.it/languages/python3) to write and test the algorithms*

I - print an array
- [x] Write an algorithm which prints everything in an array.
```
n=int(input("Please write the number of elements you want for your array: (1-10)"))
i=0
array=[]
while i < n:
    element=input("Please enter element:")
    array.append(element)
    i=i+1

print("The elements in the array are:")
for x in array:
    print("[", x,"]")
```

II - maximum
- [x] Write an algorithm which receives an array of integers and prints its **maximum**.
```
n=int(input("Please write the number of elements you want for your array: (1-10)"))
i=0
array=[]

while i < n:
    element=int(input("Please enter element:"))
    array.append(element)
    i=i+1
    
max=array[0]

for x in array:
    if x > max:
        max=x

print("The maximum element is:", max)
```

III - minimum
- [x] Write an algorithm which receives an array of integers and prints its **minimum**.
```
n=int(input("Please write the number of elements you want for your array: (1-10)"))
i=0
array=[]

while i < n:
    element=int(input("Please enter element:"))
    array.append(element)
    i=i+1

min=array[0]

for x in array:
    if x < min:
        min=x

print("The minimum element is:", min)
```

IV - minimum position
- [x] Write an algorithm which receives an array of integers and prints the position of its **minimum**.
```
n=int(input("Please write the number of elements you want for your array: (1-10)"))
i=0
array=[]

while i < n:
    element=int(input("Please enter element:"))
    array.append(element)
    i=i+1

min=array[0]

for x in array:
    if x < min:
        min=x

index=[]
for i in range(0,n):
    if array[i] == min:
        index.append(i)

print("The minimum element index is:", index)
```

V - ordered array
- [x] Write a algorithm which receives an array of integers and check if its ordered ascendantly. Print *true* if the array is ordered, *false* if it’s not.
```
n=int(input("Please write the number of elements you want for your array: (1-10)"))
i=0
array=[]

while i < n:
    element=int(input("Please enter element:"))
    array.append(element)
    i=i+1

first=array[0]
order=True
for x in array:
    if x < first:
        order=False
    first=x

if order:
    print("The elements are ordered")
else:
    print("The elements are not ordered")
```

## Resources
* [conventions](https://github.com/becodeorg/BXL-Swartz-4-27/blob/master/1.The-Field/7.Algorithmic/conventions.adoc)
* [arrays](https://computersciencewiki.org/index.php/Arrays)
