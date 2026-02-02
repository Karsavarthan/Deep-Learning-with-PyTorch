# PyTorch Basics Exercises

## AIM:
Write a Python program using PyTorch that performs the following tasks:

### Software Required:
- Python 3.x
- PyTorch
- Jupyter Notebook (for interactive development and execution)

## Algorithm:


### Step 1:

#### Name: Karsavarthan R R 
#### Register Number: 212223230100

Perform standard imports
- Import `torch` and `NumPy`.

```python
# CODE HERE
import torch
import numpy as np
```

### Step 2:
Set the random seed for NumPy and PyTorch both to `42`.

```python
# YOUR CODE HERE
seed = 42
np.random.seed(seed)
torch.manual_seed(seed)
```

### Step 3:
Create a NumPy array called `arr` that contains 6 random integers between 0 (inclusive) and 5 (exclusive).

```python
# YOUR CODE HERE
arr = np.random.randint(0, 5, size=6)
print(arr)
```

### Step 4:
Create a tensor `x` from the array above.

```python
# YOUR CODE HERE
x = torch.tensor(arr, dtype=torch.int32)
print(x)
```

### Step 5:
Change the dtype of `x` from `int32` to `int64`.

```python
# YOUR CODE HERE
x = x.type(torch.int64)
print(x)
```

### Step 6:
Reshape `x` into a `3x2` tensor.

```python
# YOUR CODE HERE
x = x.view(3, 2)
print(x)
```

### Step 7:
Return the right-hand column of tensor `x`.

```python
# YOUR CODE HERE
right_column = x[:, 1].unsqueeze(1) 
print(right_column)
```

### Step 8:
Without changing `x`, return a tensor of square values of `x`.

```python
# YOUR CODE HERE
x_squared = x ** 2
print(x_squared)
```

### Step 9:
Create a tensor `y` with the same number of elements as `x`, that can be matrix-multiplied with `x`.
- Use PyTorch directly (not NumPy) to create a tensor of random integers between 0 (inclusive) and 5 (exclusive).

```python
# YOUR CODE HERE

y = torch.randint(0, 5, (2, 3), dtype=torch.int64)
print(y)
```

### Step 10:
Find the matrix product of `x` and `y`.

```python
# YOUR CODE HERE

result = torch.matmul(x, y)
print(result)
```

## Output:

i) Import and set up PyTorch and NumPy.

![image](https://github.com/user-attachments/assets/6a6c8de4-370a-4094-9e1a-e8c094c3036e)

ii) Create and manipulate tensors.

![image](https://github.com/user-attachments/assets/40a4d58d-eb59-421d-acac-7432fe5fb6c0)

![image](https://github.com/user-attachments/assets/aaf8bd07-91e4-47e1-81a5-ee92ef45dd5a)

![image](https://github.com/user-attachments/assets/b4faf9b5-b15a-43af-99a7-adcb3f93df81)

![image](https://github.com/user-attachments/assets/9e8708f7-45ee-431f-be3b-34ee5c193108)

iii) Perform matrix operations.

![image](https://github.com/user-attachments/assets/5c402f88-ab43-4828-9f74-430a1645a850)

![image](https://github.com/user-attachments/assets/c7c547a7-cb27-48db-b13a-ea8ed109ec1c)

![image](https://github.com/user-attachments/assets/4fbb9f83-754a-4307-9c59-5d940cea9331)

![image](https://github.com/user-attachments/assets/bed85bdf-5b92-4385-bd00-239b8e643324)

## Result:
Thus, the PyTorch tensor operations, including reshaping, dtype conversion, and matrix multiplication, were successfully performed using the Python program.
