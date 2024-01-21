Sure, I'll help you convert the provided Python code into a Jupyter Notebook-friendly format. Here's the modified content:

```python
# 3.1 Data Structures and Sequences

## Tuple

A tuple is a fixed-length, immutable sequence of Python objects which, once assigned, cannot be changed. The easiest way to create one is with a comma-separated sequence of values wrapped in parentheses:

```python
tup = (4, 5, 6)
```

In many contexts, the parentheses can be omitted, so here we could also have written:

```python
tup = 4, 5, 6
```

You can convert any sequence or iterator to a tuple by invoking tuple:

```python
tuple([4, 0, 2])
```

Elements can be accessed with square brackets [] as with most other sequence types. Sequences are 0-indexed in Python:

```python
tup[0]
```

When defining tuples within more complicated expressions, it’s often necessary to enclose the values in parentheses, as in this example of creating a tuple of tuples:

```python
nested_tup = (4, 5, 6), (7, 8)
```

While the objects stored in a tuple may be mutable themselves, once the tuple is created it’s not possible to modify which object is stored in each slot:

```python
tup = tuple(['foo', [1, 2], True])
# This will raise a TypeError
tup[2] = False
```

If an object inside a tuple is mutable, such as a list, you can modify it in place:

```python
tup[1].append(3)
```

You can concatenate tuples using the + operator to produce longer tuples:

```python
(4, None, 'foo') + (6, 0) + ('bar',)
```

Multiplying a tuple by an integer, as with lists, has the effect of concatenating that many copies of the tuple:

```python
('foo', 'bar') * 4
```

Unpacking tuples:

```python
tup = (4, 5, 6)
a, b, c = tup
```

For more examples and details, please refer to the original code.

## List

In contrast with tuples, lists are variable length and their contents can be modified in place. Lists are mutable. You can define them using square brackets [] or using the list type function:

```python
a_list = [2, 3, 7, None]
tup = ("foo", "bar", "baz")
b_list = list(tup)
```

Adding and removing elements:

```python
b_list.append("dwarf")
b_list.insert(1, "red")
b_list.pop(2)
b_list.remove("foo")
```

For more examples and details, please refer to the original code.

## Dictionary

The dictionary or dict may be the most important built-in Python data structure. In other programming languages, dictionaries are sometimes called hash maps or associative arrays.

```python
empty_dict = {}
d1 = {"a": "some value", "b": [1, 2, 3, 4]}
```

Accessing, inserting, or setting elements:

```python
d1[7] = "an integer"
d1["b"]
del d1[5]
d1.pop("dummy")
```

For more examples and details, please refer to the original code.

## Set

A set is an unordered collection of unique elements.

```python
set([2, 2, 2, 1, 3, 3])
{2, 2, 2, 1, 3, 3}
```

Set operations:

```python
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7, 8}
a.union(b)
a.intersection(b)
a.difference(b)
a.symmetric_difference(b)
```

For more examples and details, please refer to the original code.

# Built-In Sequence Functions

## enumerate

It’s common when iterating over a sequence to want to keep track of the index of the current item. Python has a built-in function, enumerate:

```python
for index, value in enumerate(collection):
    # do something with value
```

## sorted

The sorted function returns a new sorted list from the elements of any sequence:

```python
sorted([7, 1, 2, 6, 0, 3, 2])
sorted("horse race")
```

## zip

zip “pairs” up the elements of a number of lists, tuples, or other sequences:

```python
seq1 = ["foo", "bar", "baz"]
seq2 = ["one", "two", "three"]
zipped = zip(seq1, seq2)
```

## reversed

reversed iterates over the elements of a sequence in reverse order:

```python
list(reversed(range(10)))
```

For more examples and

 details, please refer to the original code.
```

Feel free to ask if you have any questions or if there's anything specific you'd like to discuss!
