# Learn Python

Read Allen Downey's [Think Python](http://www.greenteapress.com/thinkpython/) for getting up to speed with Python 2.7 and computer science topics. It's completely available online, or you can buy a physical copy if you would like.

<a href="http://www.greenteapress.com/thinkpython/"><img src="img/think_python.png" style="width: 100px;" target="_blank"></a>

For quick and easy interactive practice with Python, many people enjoy [Codecademy's Python track](http://www.codecademy.com/en/tracks/python). There's also [Learn Python The Hard Way](http://learnpythonthehardway.org/book/) and [The Python Tutorial](https://docs.python.org/2/tutorial/).

---

### Q1. Lists &amp; Tuples

How are Python lists and tuples similar and different? Which will work as keys in dictionaries? Why?

>> Lists are mutable but tuples are not. Tuples bececause [lists cannot provide a valid hash method](https://wiki.python.org/moin/DictionaryKeys)

---

### Q2. Lists &amp; Sets

How are Python lists and sets similar and different? Give examples of using both. How does performance compare between lists and sets for finding an element. Why?

>> Both represent an union of elements. 
`set`: Unordered collections of unique elements
```a = set('apple')
   b = set('banana')
   a-b
```
`lists`: ordered collections of elementsf
``` squares = []
    for x in range(10):
       squares.append(x**2)
```
Set is faster to determine if an element is in a set.
---

### Q3. Lambda Function

Describe Python's `lambda`. What is it, and what is it used for? Give at least one example, including an example of using a `lambda` in the `key` argument to `sorted`.

>> [While normal functions are defined using the def keyword, in Python anonymous functions are defined using the lambda keyword.](https://www.programiz.com/python-programming/anonymous-function)
```
mylist = [3,6,3,2,4,8,23]
sorted(mylist, key=lambda x: x%2==0)
```
[interesting intro](https://stackoverflow.com/questions/8966538/syntax-behind-sortedkey-lambda)

---

### Q4. List Comprehension, Map &amp; Filter

Explain list comprehensions. Give examples and show equivalents with `map` and `filter`. How do their capabilities compare? Also demonstrate set comprehensions and dictionary comprehensions.

>> map:```number_list = list(range(100))```
```
square_list = map(lambda x: x**2, number_list)
square_list = [x**2 for x in numbers]
```
filter:
```
odd_list = filter(lambda x: 2x+1, number_list)
odd_list = [2x+1 for x in number_list]
```
set comprehension
```{x for x in 'abracadabra' if x not in 'abc'}```
dictionary comprehension 
```{x: x**2 for x in (2, 4, 6)}
```
[intereseint example](http://www.diveintopython3.net/comprehensions.html)
```
{value:key for key, value in a_dict.items()}
```
[read this](https://martin-thoma.com/python-map-reduce-filter/) and [this](https://docs.python.org/3/tutorial/datastructures.html)

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





