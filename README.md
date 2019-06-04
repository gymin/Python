# Introduction to Python

## Data structure 

### List and Membership Operators 

#### List: a data type for mutable ordered sequence of elements 

```
months = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']

print(month[0])
```
>> January 

```
print(month[-1])
```
>> December 
```
months[len(months) - 1] 
```
>>> December 

Slicing: using indices to slice off parts of an object like a string or a list 

```
q3 = months[6:9] # first: lower bound (inclusive), second: upper bound (exclusive) 
print(q3)
```
>> July, August, September
```
first_half = months[:6]
print(first_half)
```
>> Janunary, February, March, April, May, June 

List is a type (like string, int, but very close to strings) 
Strings are sequences of letters, while list elements can be any type of object 
List can be modified bu strings can't be

#### Membership operators 

- `in`: evaluates if object on left side is included in object on right side 
- `not in`: evaluates if object on left side is _not_ included in object on right side 

```
print('Sunday' in months, 'Sunday' not in months) 
```
>> False True 

### Mutability and Order 

#### Mutability 
Whether or not we can change an object once it has been created. If an object (like a list or string) can be changed (e.g. like list), then it's called _mutable_. 
If an object cannot be changed with creating a completely new object (e.g. like strings), then the object is considered _immutable_

E.g. list 
```
months[3] = 'Friday' 
print(months) 
```
>> January, February, March, Friday, May, June, July, August, September, October, November, December 

e.g. Strings 
```
greeting = "Hello there~
greetig[3] = 'i'
print(greeting) 
```
>> TypeError: 'str' object does not support item assignment 

#### Order 
Whether the position of an element in the object can be used to acess the element (e.g. index is possible)
Both strings and lists are _ordered_

### List methods 

```
scores = ["B", "C", "A", "D", "B", "A"]
grades = scores 
print("scores: " + scores)
print("grades: " + grades_ 
score[3] = "B" 
print("scores: " + scores)
print("grades: " + grades_ 
```
>>> Scores: ["B", "C", "A", "D", "B", "A"]
grades: ["B", "C", "A", "D", "B", "A"]
scores: ["B", "C", "A", **"B"**, "B", "A"]
grades: ["B", "C", "A", **"B"**, "B", "A"]

`len()`: Returns how many elements are in a list 
`max()`: Returns the greatest element of a list (e.g. largest number, or the element that woud occur last if the list was sorted alphabetically) - as long as they are comparable
`min()`: Returns the smallest element 
`sorted()`: Returns a copy of a list in order from smallest to largest, leaving the list unchanged 
