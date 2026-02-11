# Using SageMath with Jupyter in VS Code

## Creating a Notebook

- Open VS Code
- Create a new Jupyter Notebook (.ipynb)
- Select the kernel:
  SageMath (conda env: sage)

## Test Code

```python
var('r')
f = function('f')(r)
diff(f, r, 2)

