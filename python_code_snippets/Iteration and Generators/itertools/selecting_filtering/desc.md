### Selecting and Filtering

```
itertools.filterfalse

it retains elements where the predicate evaluates to false

Example:
    filterfalse(lambda x: x < 4, [1, 10 ,2, 10, 3, 10])

    yields -> [10, 10, 10]

    filterfalse(None, [0, '', 'hello', False])

    yields -> [0, '', False]

```

```

itertools.compress

a way of filtering, using the truthiness of item in another iterable

Example:
    data = ['a', '', 'b', 'c', 'e']
    selectors = [True, 1, False, 0, 5]

    compress(data, selectors)
    yields -> ['a', 'e']

```

```

itertools.takewhile

returns an iterator that will yield items while pred(item) is Truthy

Example:
    takewhile(lambda x: x < 5, [1, 3, 5, 2, 1])

    yields -> [1, 3]

```

```
itertools.dropwhile

returns an iterator that will yield items while pred(item) is Falsy

Example:
    takewhile(lambda x: x < 5, [1, 3, 5, 2, 1])

    yields -> [5, 2, 1]
