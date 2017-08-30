# Learn Python

Read Allen Downey's [Think Python](http://www.greenteapress.com/thinkpython/) for getting up to speed with Python 2.7 and computer science topics. It's completely available online, or you can buy a physical copy if you would like.

<a href="http://www.greenteapress.com/thinkpython/"><img src="img/think_python.png" style="width: 100px;" target="_blank"></a>

For quick and easy interactive practice with Python, many people enjoy [Codecademy's Python track](http://www.codecademy.com/en/tracks/python). There's also [Learn Python The Hard Way](http://learnpythonthehardway.org/book/) and [The Python Tutorial](https://docs.python.org/2/tutorial/).

---

### Q1. Lists &amp; Tuples

How are Python lists and tuples similar and different? Which will work as keys in dictionaries? Why?

>> Lists and tuples are similar because they both store elements, maintain their order, and can have elements of any type. They're different because tuples are immutable whereas lists are mutable, use () while lists use [], and tuples generally contain elements that represent different concepts while lists have elements that represent similar concepts. 

Tuples can work as keys in dictionaries because they cannot be changed.

---

### Q2. Lists &amp; Sets

How are Python lists and sets similar and different? Give examples of using both. How does performance compare between lists and sets for finding an element. Why?

>> Lists and sets are similar because they both store elements of different data types. They're different because sets are unordered, immutable, can't have any duplicates, and require their elements to be hashable. 

It is faster to find an element in a set because you don't have to iterate through each element to find the requested one. Rather, since the hash function outputs the hash value that represents the input's position in the set, it just needs to check to see if the input is at the position determined by the hash. Thus, the size of the set doesn't matter with regards to the speed of this process.

---

### Q3. Lambda Function

Describe Python's `lambda`. What is it, and what is it used for? Give at least one example, including an example of using a `lambda` in the `key` argument to `sorted`.

>> Lambda is a way to create a temporary function that you only need for that particular instance. 

x = [(1,7), (1,3), (3,4,5), (2,2)]
x.sort(key = lambda x: x[1])

y = lambda x: x/2
y = lambda x: x**2

---

### Q4. List Comprehension, Map &amp; Filter

Explain list comprehensions. Give examples and show equivalents with `map` and `filter`. How do their capabilities compare? Also demonstrate set comprehensions and dictionary comprehensions.

>> List comprehensions are a concise way to create lists based off a pre-existing list. 

x = [1, 2, 4, 5, 7, 8, 10, 12, 14]
[(i**3) / 2 for i in x]
list(map(lambda x: x**3 / 2, x))

[i for i in x if i % 4 == 0]
list(filter(lambda x: x % 4 == 0, x))

If you're calling an already-defined function on each element, map() is faster than list comprehension. But when evaluating a random expression, list comprehension is faster than using map() because map() incurs an extra function call for each element.

Set Comprehensions:

{s**2 for s in range(10)}
{s for s in range(3,33) if s % 4 == 0}

Dictionary Comprehensions:
{y: x**2 for (y, x) in zip(string.ascii_lowercase, range(26))}
{x: x**3 for x in range(10)}
---

### Complete the following problems by editing the files below:

### Q5. Datetime
Use Python to compute days between start and stop date.   
a.  

```
date_start = '01-02-2013'    
date_stop = '07-28-2015'
```

>> REPLACE THIS TEXT WITH YOUR RESPONSE (answer will be in number of days)

b.  
```
date_start = '12312013'  
date_stop = '05282015'  
```

>> REPLACE THIS TEXT WITH YOUR RESPONSE (answer will be in number of days)

c.  
```
date_start = '15-Jan-1994'      
date_stop = '14-Jul-2015'  
```

>> REPLACE THIS TEXT WITH YOUR RESPONSE  (answer will be in number of days)

Place code in this file: [q5_datetime.py](python/q5_datetime.py)

---

### Q6. Strings
Edit the 7 functions in [q6_strings.py](python/q6_strings.py)

---

### Q7. Lists
Edit the 5 functions in [q7_lists.py](python/q7_lists.py)

---

### Q8. Parsing
Write a script as indicated (using the football data) in [q8_parsing.py](python/q8_parsing.py)





