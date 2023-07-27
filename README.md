import numpy as np

def solve_system_of_equations(A, b):
  """
  Solves the system of equations Ax = b for x.

  Args:
    A: The coefficient matrix.
    b: The constant vector.

  Returns:
    x: The solution vector.
  """

  inverse = np.linalg.inv(A)
  x = inverse * b

  return x

A = np.array([[2, 5], [1, 3]])
b = np.array([[7], [5]])

x = solve_system_of_equations(A, b)

print(x)
