# Introdcution to Python

## Say "Hello, World!" With Python

```

print("Hello, World!")

```

## Python If-Else

```

# if statement use
n = int(input(''))
if n%2 == 1 : 
    print('Weird')
elif n >= 2 and n <= 5 :
    print('Not Weird')
elif n >= 6 and n <= 20 :
    print('Weird')
elif n >= 20 :
    print('Not Weird')

```

## Arithmetic Operators

```

a = int(input(''))
b = int(input(''))
print(a+b)
print(a-b)
print(a*b)

```

## Python: Division

```

a = int(input(''))
b = int(input(''))
c = int(a/b)
d = float(a/b)
print(c)
print(d)

```

## Loops

```

n = int(input(''))
for i in range(n):
    print(i**2)

```

## Write a function

```

def is_leap(year):
    if year%400 == 0 and year%100 == 0:
        return True
    elif year%100 == 0:
        return False
    elif year%4 == 0:
        return True
    else:
        return False

```

## Print Function

```

n = int(input())
for i in range(1, n+1) : 
    print(i, end = "")

```
