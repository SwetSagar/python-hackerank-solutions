# Itertools 

Used for permutation and combination in Python

## itertools.product()

```


from itertools import product

A = map(int, input().split())
B = map(int, input().split())

C = list(product(A,B))

for item in C : 
    print(item, end=' ')


```

## itertools.permutations() 

```
from itertools import permutations

A,B = input().split()
B = int(B)
## A = HACK and B = 3

for p in sorted(permutations(A,B)):
    print(''.join(p))

```

## itertools.combinations()

```

from itertools import combinations

M, N = map(str, input().split())
M = sorted(M)
N = int(N)

for i in range(1,N+1) : 
    for comb in combinations(M, i):
        print(''.join(comb))

```

## itertools.combinations_with_replacement()

```

from itertools import combinations_with_replacement

M, N = map(str, input().split())
M = sorted(M)
N = int(N)

for comb in combinations_with_replacement(M,N):
    print(''.join(comb))

```

## Compress the String!

```


```


## Iterables and Iterators


```

```


## Maximize It! 

```


```
