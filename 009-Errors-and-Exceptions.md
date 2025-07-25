# Errors and Exceptions

## Exceptions 

```

T = int(input())

for _ in range(T):
    a, b = input().split()
    try:
        print(int(a)//int(b))
    except (ZeroDivisionError, ValueError) as e:
        print("Error Code:",e)

```

## Incorrect Regex 

```

- [ ] #todo

```

