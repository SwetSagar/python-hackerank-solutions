# Collections Module

## collections.Counter()

```

from collections import Counter

X = int(input())
shoe_size_list = list(map(int, input().split()))
N_customers = int(input())
inventory = Counter(shoe_size_list)
total_price = 0

for _ in range(N_customers):
    size, price = map(int, input().split())
    if inventory[size] > 0 : 
        total_price += price
        inventory[size] -= 1

print(total_price)

```

## DefaultDict Tutorial 

```


from collections import defaultdict
N,M = map(int, input().split())
d = defaultdict(list)

#group A list 
for i in range(1, N+1):
    d[input()].append(i)

#group B query
for j in range(M):
    word = input()
    if word in d:
        print(' '.join(map(str, d[word])))
    else:
        print(-1)

```

## Collections.namedtuple() 

```

from collections import namedtuple

N = int(input())
fields = input().split()
Student = namedtuple('Student', fields)
total_marks = 0

for _ in range(N) : 
    row = input().split()
    student = Student(*row)
    total_marks += int(student.MARKS)
    
print(f"{total_marks / N:.2f}")

```

## Collections.OrderedDict()

```

from collections import OrderedDict

N = int(input())
req_dict = OrderedDict()

for _ in range(N):
    name, price = input().rsplit(' ', 1)
    price = int(price)
    item_name = name
    if item_name in req_dict :
        req_dict[item_name] += price
    else :
        req_dict[item_name] = price

for name,price in req_dict.items() :
    print(name, price)

```

## Collections.deque()

```

from collections import deque
d = deque()
N = int(input())

for _ in range(1, N+1):
    cmd = input().split()
    if cmd[0] == 'append':
        d.append(int(cmd[1]))
    if cmd[0] == 'appendleft':
        d.appendleft(int(cmd[1]))
    if cmd[0] == 'pop':
        d.pop()
    if cmd[0] == 'popleft':
        d.popleft()

print(*d)

```


## Word Order

```

- [ ] #todo

```

## Company Logo

```

- [ ] #todo

```

## Piling Up!


```

- [ ] #todo

```


