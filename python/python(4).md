# Function

> It is bundle of doing specific work.

![image-20200725175829103](Python(4).assets/image-20200725175829103.png)

### 1. Why do we use function?

- It is more readable.
- It is more reusable.
- It is more comfortable that maintain and manage code.



### 2. Definition/call of function

- It is defined by `def {} :`.
- It can transmit parameter.
- It can transmit result value by using `return` . If does not use `return` , return `None`.

```python
def function_name(parameter1, parameter2) :
    pass
	return value
```



### 3. Output of function

- If it is used `return` , it can return any object. It is possible only object.

- If the function is ended, it goes back to the place called function.



### 4. Input of function

- Parameter

  ```python
  def func(x) :
      return x+2
  ```

  - `x` is parameter. This is same variable transmitted input value and used in function.

- Argument

  - It is input value transmitted to function.
  - It is used when you call the function.

  ```python
  func(2) # --> argument is '2'
  ```

- Positional argument

  - The function is judge argument through that of place.

- Default argument values

  - When the function is called, it is possible that you can set argument value.
  - It is impossible that you use positional argument after using default argument.

  ```python 
  def func(name='홍길동',age): # --> (age, name='홍길동')
      pass
  ```

- Keyword argument

  - It is possible that you can transfer specific argumetnt through name of value.
  - It is impossible that you use positional argument after using keyword argument.

  ```python
  func(name='김지형',age=26) # --> O
  func(age=26,'김지형') # --> X
  ```

- Arbitrary argument list

  - For you transfer many arguments, you can use arbitrary argument list.
  - Arbitrary argument list is used tuple, you must write `'*'` before value name.

  ```python
  def func(a,b,*args)
  ```

- Arbirary keyword argument

  -  Arbitrary keyword list name is used to `'kwargs'` , you must write `'**'` before value name.

  ```python
  def func(**kwargs):
      pass
  func(name='김지형',age=26)
  ```

  