# Three ways to code dictionary in python

## 1st way: normal way
```python
bob = {'name': 'Bob Smith', 'age': 42, 'pay': 30000, 'job': 'dev'}
sue = {'name': 'Sue Johns', 'age': 45, 'pay': 40000, 'job': 'hdw'}
```

## 2nd way: using dict()
```python
bob = dict(name='Bob Smith', age=42, pay=30000, job='dev')
sue = dict(name='Sue Johns', age=45, pay=40000, job='hdw')
```

## 3rd way: using zip()
```python
labels = ['name', 'age', 'pay', 'job']
values = ['Sue Johns', 45, 40000, 'hdw']

sue = dict(zip(labels, values))
```
## additional way: giving default values
```python
fields = ('name', 'age', 'job', 'pay')
record = dict.fromkeys(fields, '?')
```
#### result:
```python
>>> record
{'job': '?', 'pay': '?', 'age', 'name': '?'}
```

