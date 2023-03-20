### Infinite Iterators

```
itertools.count

-> start, step
-> NO STOP
-> infinite


count(10, 2) -> 10, 12, 14 ...
count(10.5, 0.1) -> 10.5, 10.6, 10.7 ...

takewhile(lambda x: x < 10.8, count(10.5, 0.1)) -> 10.5, 10.6, 10.7 ...

```

```
itertools.cycle

allows is to loop over a finite iterable indefinitely

Example:
    cycle(['a', 'b', 'c']) 
    yields -> ''a', 'b', 'c', 'a', 'b', 'c' ...

    it supports iterators to cycle infinitely

```

```
itertools.repeat

yields the same value indefinitely

Example:
    repeat('spam') -> 'spam', 'spam', 'spam' ...

optionally, you can specify a count to make the iterator finite

Example:
    repeat('spam', 4) -> 'spam', 'spam', 'spam', spam'

Caveat:
    the items yielded by repeat are the same object

```