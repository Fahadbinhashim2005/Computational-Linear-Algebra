## Pseudocode for linear algebra
```python
FUNCTION matrix_sum(A,B);
  Get the no of rows and columns in matrix A
  Create an empty matrix C with same dimension 
  FOR each row i;
    FOR each column j;
      Set C[i][j] to the sum of A[i][j] and B[i][j]
  Return the matrix C
END FUNCTION

## Pseudocode for linear algebra
```python
FUNCTION matrix_sum(A,B);
  Create Augmented matrix:K=[A|B]
  Reduce in Row Reduced Echelon form
  Rank=no of non zero rows of RREF
  IF Rank(K)!=Rank(A):
    print(System is inconsistent)
  ELSEIF
    print(Solve using back substitution)   
