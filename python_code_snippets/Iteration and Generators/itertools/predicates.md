### Predicates

```
A function that takes a single argument and returns True or False
is called a predicate
```

```
We can make __any__ and __all__ more useful by first applying a predicate to each element of the iterable
```

```
sample predicate

pred = lambda x: x < 10

application:

results = [pred(1), pred(2), pred(3), pred(4), pred(100)]
```