In this exercise, you'll practice converting between numeric types and observe how different conversion methods work.

# Instructions

At each stage, use `print()`{.python} statements to check your results:

1. Create a variable named `my_number`{.python} and set its value to `2.6`{.python}
2. Create a variable named `round_down`{.python} which is `my_number`{.python} converted to an int (rounded toward zero)
3. Create a variable named `round_nearest`{.python} which is `my_number`{.python} rounded to the nearest integer
4. Create a variable named `new_float`{.python} which is `round_nearest`{.python} converted back to a float
5. Change the value of `my_number`{.python} to `-3.6`{.python} and re-run your code to see how the conversion functions behave with negative numbers

# Code Template

Begin with this template and fill in the missing conversions:

```py-cell
# Create my_number
my_number =
print(my_number)

# Create round_down
round_down =
print(round_down)

# Create round_nearest
round_nearest =
print(round_nearest)

# Create new_float
new_float =
print(new_float)
```

# Questions to Consider

* What is the difference between `int()`{.python} and `round()`{.python}?
* How do they behave differently with negative numbers?
* Can you always convert a float to an int and back without losing information?

# Sample Solution

Click below to reveal a sample solution

>[!HIDDEN]
> Let's practice converting between numeric types in Python, step by step.
>
> ```py-cell
> # Start with a float
> my_number = 2.6
> print(my_number)
> ```
>
> Convert the float to an integer using `int()` (truncates toward zero).
> 
> ```py-cell
> round_down = int(my_number)
> print(round_down)
> ```
>
> Round to the nearest integer using `round()`.
>
> ```py-cell
> round_nearest = round(my_number)
> print(round_nearest)
> ```
>
> Convert the rounded integer back to a float.
>
> ```py-cell
> new_float = float(round_nearest)
> print(new_float)
> ```
>
> Now let's try the same steps with a negative number.
>
> ```py-cell
> my_number = -3.6
> print(my_number)
> round_down = int(my_number)
> print(round_down)
> round_nearest = round(my_number)
> print(round_nearest)
> new_float = float(round_nearest)
> print(new_float)
> ```
>
> ## Answers to Question
>
> * `int()`{.python} truncates towards zero, whilst `round()`{.python} rounds to the nearest integer.
> * `round()`{.python} always rounds to the nearest number. `int()`{.python} will round down for positive numbers and up for negative numbers (both toward zero).
> * If you convert a float to an integer, you will lose the decimal part of the number so, even after converting back to a float, the value will be different from the original (unless the original number was already a whole number).
