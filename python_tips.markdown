# Some Python tips and tricks

Wisdom from [Tim Peters](https://youtu.be/1wAOy88WxmY):


```python
import this
```

    The Zen of Python, by Tim Peters
    
    Beautiful is better than ugly.
    Explicit is better than implicit.
    Simple is better than complex.
    Complex is better than complicated.
    Flat is better than nested.
    Sparse is better than dense.
    Readability counts.
    Special cases aren't special enough to break the rules.
    Although practicality beats purity.
    Errors should never pass silently.
    Unless explicitly silenced.
    In the face of ambiguity, refuse the temptation to guess.
    There should be one-- and preferably only one --obvious way to do it.
    Although that way may not be obvious at first unless you're Dutch.
    Now is better than never.
    Although never is often better than *right* now.
    If the implementation is hard to explain, it's a bad idea.
    If the implementation is easy to explain, it may be a good idea.
    Namespaces are one honking great idea -- let's do more of those!


### 1. You can use `_` interactively


```python
4 + 6
```




    10




```python
_ + 5
```




    15



### 2. Working with references


```python
a = [[1, 2, 3, 4, 5]] * 4
a[0][0] = 0
```


```python
a
```




    [[0, 2, 3, 4, 5], [0, 2, 3, 4, 5], [0, 2, 3, 4, 5], [0, 2, 3, 4, 5]]



### 3. Create dictionary from two lists


```python
keys = ["key_1", "key_2", "key_3"]
values = [1, 2, 3]
my_dict = dict(zip(keys, values))
print(my_dict)
```

    {'key_1': 1, 'key_2': 2, 'key_3': 3}


### 4. Merge dictionaries with `**`


```python
my_dict_1 = {"name": "Alice", "gender": "F"}
my_dict_2 = {"name": "Alice", "age": 29, "occupation": "lawyer"}
merged_dict = {**my_dict_1, **my_dict_2}
print(merged_dict)
```

    {'name': 'Alice', 'gender': 'F', 'age': 29, 'occupation': 'lawyer'}


### 5. String formatting


```python
name = "Alice"
occupation = "lawyer"
my_string = "{} is a {}".format(name, occupation)
print(my_string)
```

    Alice is a lawyer



```python

```
