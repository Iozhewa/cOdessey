# 98 Qs of Python: A cOddessey
Join me as I avoid project-based learning, and find some algorithmic nuance in Programmiz's Python examples.<br>
I will be treating them as questions, and attempt to solve them without reading their solution code (at first). My goal is to learn something new, do something quick, and have some fun.

## Q1: Hello, World!
Alright, fairly simple. [W3Schools](https://www.w3schools.com/python/python_lambda.asp) is what I used to revise the use of a Lambda function.
<details>

  ``` python
  greetings = lambda x: print("Hello, world!")
  greetings(0)
  ```
  For each solve, I will be offering a solution wrapped in a function. Whether or not that will balooon into dependent functions and classes, who's to say.<br><br>
  Here, we have a cheeky anonymous function, for a print statement that will execute regardless of what you parse through.<br>

  ``` shell
  Hello, world!
  ```
</details>

## Q2: Add Two Numbers!
Also simple, but we'll use lambda traditionally :p
<details>

  ``` python
  sums = lambda x, y: print(f"{x} + {y} = {int(x)+int(y)}")
  sums(input("Enter addend (1/2): "), input("Enter addend (2/2): "))
  ```
  This early into the markdown, I don't want to get too particular with inputs. At the same time, I want to tie in loose ends. That's a normal thing to want, right?<br><br> 
  Here, our anonymous function relies on explicit type conversion to work in the given f-string. So that I can just hint to that, I hide under the technical jargon of 'addend' and 'x/2 capacity'.<br>

  ``` shell
  Enter addend (1/2): 1
  Enter addend (2/2): 2
  1 + 2 = 3
  ```
</details>

## Q3: Find the Square Root!
Now this is interesting, because it can be solved with the consequences of the index laws.
<details>

  ``` python
  squareRoot = lambda x: print("Root is:", int(x)**0.5)
  squareRoot(input("Present an integer for its square root: "))
  ```
  The exponent operator in python is `**`, which like many operators, is not limited to integers. The opposite of a square number is found by the inverse of `2`, which leads us to `x^0.5`. <br><br>
  Something important to mention here is that I mistakenly started coding with a fraction, `1/2`. This is itself an operation! The rules of PEMDAS/BIDMAS still boggle me in little ways, it seems. Moral of the story: Fraction bad, Decimal gooood<br>

  ``` shell
  =====TEST 1=====
  Present an integer for its square root: 16
  Root is: 4.0

  =====TEST 2=====
  Present an integer for its square root: 8
  Root is: 2.8284271247461903
  ```
</details>
