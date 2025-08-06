# PyTorch Basics Exercises
## Name: Ezhil Nevedha.K
## Reg.no : 212223230055
## AIM:
Write a Python program using PyTorch that performs the following tasks:

### Software Required:
- Python 3.x
- PyTorch
- Jupyter Notebook (for interactive development and execution)

## Algorithm:

### Step 1:
Perform standard imports
- Import `torch` and `NumPy`.

```python
import torch
import numpy as np
```

### Step 2:
Set the random seed for NumPy and PyTorch both to `42`.

```python
np.random.seed(42)
torch.manual_seed(42)
```

### Step 3:
Create a NumPy array called `arr` that contains 6 random integers between 0 (inclusive) and 5 (exclusive).

```python
arr = np.random.randint(0, 5, size=6)
print(arr)
```

### Step 4:
Create a tensor `x` from the array above.

```python
x = torch.from_numpy(arr)
print(x)
```

### Step 5:
Change the dtype of `x` from `int32` to `int64`.

```python
x = x.type(torch.int64)
print(x)
```

### Step 6:
Reshape `x` into a `3x2` tensor.

```python
x = x.reshape(3, 2)
print(x)
```

### Step 7:
Return the right-hand column of tensor `x`.

```python
right_col = x[:, 1]
print(right_col)
```

### Step 8:
Without changing `x`, return a tensor of square values of `x`.

```python
squ = x**2
print(squ)
```

### Step 9:
Create a tensor `y` with the same number of elements as `x`, that can be matrix-multiplied with `x`.
- Use PyTorch directly (not NumPy) to create a tensor of random integers between 0 (inclusive) and 5 (exclusive).

```python
y = torch.randint(0, 5, (2, 3))
print(y)
```

### Step 10:
Find the matrix product of `x` and `y`.

```python
y = torch.randint(0, 5, (2, 3), dtype=x.dtype)
res = x @ y
print(res)
```

## Output:
i) Import and set up PyTorch and NumPy.
<img width="307" height="93" alt="image" src="https://github.com/user-attachments/assets/e69f7140-d354-42bc-adb1-6badacbb6a74" />

ii) Create and manipulate tensors.
<img width="519" height="345" alt="image" src="https://github.com/user-attachments/assets/7d6d26a2-525a-427b-a7a5-405049c44941" />

iii) Perform matrix operations.
<img width="737" height="587" alt="image" src="https://github.com/user-attachments/assets/0e26107c-c017-4aa4-9837-6a6e228d7516" />


## Result:
Thus, the PyTorch tensor operations, including reshaping, dtype conversion, and matrix multiplication, were successfully performed using the Python program.
