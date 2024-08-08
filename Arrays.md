# Array in Python

In Python, arrays can be implemented using lists from the standard library or using the `array` module for more efficient storage of elements of the same type.

## Example of Arrays using Lists

### Array for Integral Value
```
# Declaration and Initialization
A = [2, 5, 8, 44, 21, 11, 7, 9, 3, 1]

# Accessing elements
print(A[0])  # Output: 2
print(A[3])  # Output: 44
```

### Array for Character Value
```
# Declaration and Initialization
B = ['f', 'd', 'a', 'b', 'n', 'j', 'l', 's', 'e', 'y']

# Accessing elements
print(B[0])  # Output: f
print(B[4])  # Output: n
```

### Example of Arrays using the array Module

```
# Importing the array Module
import array
```

#### Array for Integral Value
```
# Declaration and Initialization
A = array.array('i', [2, 5, 8, 44, 21, 11, 7, 9, 3, 1])

# Accessing elements
print(A[0])  # Output: 2
print(A[3])  # Output: 44
```

#### Array for Character Value
```
# Declaration and Initialization
B = array.array('u', 'fdabnjlse')
# Note: 'u' is for Unicode characters

# Accessing elements
print(B[0])  # Output: f
print(B[4])  # Output: n
```

## Multi-Dimensional Arrays using Lists

Two-Dimensional Array
```
# Declaration and Initialization
arr = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]

# Accessing elements
print(arr[0][0])  # Output: 1
print(arr[1][2])  # Output: 6
```

Three-Dimensional Array
```
# Declaration and Initialization
arr = [
    [
        [1, 2, 3],
        [4, 5, 6]
    ],
    [
        [7, 8, 9],
        [10, 11, 12]
    ]
]

# Accessing elements
print(arr[0][0][0])  # Output: 1
print(arr[1][1][2])  # Output: 12
```

> Note: Python can store integers and strings in the same array unlike Java and C++

## Advantages of Arrays in Python
- Dynamic sizing with lists.
- Easy to use and initialize.
- Lists can store different data types.

## Disadvantages of Arrays in Python
- Python lists are not as memory efficient as arrays in other programming languages.
- Requires using the array module for type-specific arrays, which is less common.

# Big O Notation:

Lookup by index = O(1)
Lookup by value = O(n)
Array traversal = O(n)
Array insertion = O(n)
Array deletion = O(n)

