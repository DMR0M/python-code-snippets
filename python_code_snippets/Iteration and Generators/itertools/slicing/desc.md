### Slicing
```
itertools.islice

islice(iterable, start, stop(required), step)

```

```
from itertools import islice

l = (n for n in range(1, 11))

result = islice(l, 1, 3)

```

```
These are lazy iterators
```

