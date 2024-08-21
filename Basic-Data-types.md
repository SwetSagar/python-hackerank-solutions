# Basic Data Types

## List Comprehensions

```
# List comprehension nested 
x = int(input(''))
y = int(input(''))
z = int(input(''))
n = int(input(''))
list1 = [[i,j,k] for i in range(x+1) for j in range(y+1) for k in range(z+1) if i+j+k != n]
print(list1

```

## Find the Runner-Up Score!

```

n = int(input())
arr = list(map(int, input().split()))
arr.sort()

new_list = set(arr)
new_list.remove(max(new_list))
print(max(new_list))

```

## Nested Lists

```

if __name__ == '__main__':
    data = []
    ans = []
    for _ in range(int(input())):
        name = input()
        score = float(input())
        data.append([name, score])
        ans.append(score)
    
    data.sort()
    ans = sorted(list(set(ans)))
    ans.remove(min(ans))
    for x in range(len(data)):
        if data[x][1] == min(ans):
            print(data[x][0])

```

## Finding the percentage

```

if __name__ == '__main__':
    n = int(input())
    student_marks = {}
    for _ in range(n):
        name, *line = input().split()
        scores = list(map(float, line))
        student_marks[name] = scores
    query_name = input()
    average = sum(student_marks[query_name])/ len(student_marks[query_name])
    print(format(average,".2f"))

```

## Lists

```

if __name__ == '__main__':
    N = int(input())
    my_list = []

    for _ in range(N):
        command = input().split()

        if command[0] == "insert":
            my_list.insert(int(command[1]), int(command[2]))
        elif command[0] == "print":
            print(my_list)
        elif command[0] == "remove":
            my_list.remove(int(command[1]))
        elif command[0] == "append":
            my_list.append(int(command[1]))
        elif command[0] == "sort":
            my_list.sort()
        elif command[0] == "pop":
            my_list.pop()
        elif command[0] == "reverse":
            my_list.reverse()

```

## Tuples

```

if __name__ == '__main__':
    n = int(input())  # Number of elements in the tuple
    integer_list = map(int, input().split())  # Space-separated integers as input

    # Create a tuple from the input integers
    my_tuple = tuple(integer_list)

    # Calculate and print the result of hash(tuple)
    result = hash(my_tuple)
    print(result)

```

