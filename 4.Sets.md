# Sets

## Introduction to Sets

```
def average(array):
    # your code goes here
    return sum(set(array))/len(set(array))

```

## No Idea!

```

# Enter your code here. Read input from STDIN. Print output to STDOUT

space_separated_int = input()
space_separated_n = input()
space_separated_mA = input()
space_separated_mB = input()

x = list(map(int, space_separated_n.split()))
y = set(map(int, space_separated_mA.split()))
z = set(map(int, space_separated_mB.split()))

happiness = 0

for integer in x :
    if integer in y:
        happiness += 1
    elif integer in z :
        happiness -= 1
    
        
print(happiness)

```

## Symmetric Difference

```

# Enter your code here. Read input from STDIN. Print output to STDOUT
M = int(input())
space_separated_M = input()
N = int(input())
space_separated_N = input()


M_set = set(map(int, space_separated_M.split()))

N_set = set(map(int, space_separated_N.split()))

diff = sorted(M_set.symmetric_difference(N_set))
for num in diff:
    print(num)

```

## Set .add()

```

# Enter your code here. Read input from STDIN. Print output to STDOUT

n = int(input())
country_set = set()

while n > 0 :
    country = str(input())
    n -= 1
    country_set.add(country)

print(len(country_set))

```

## Set .discard(), .remove() & .pop()

```

elements_inset_n = int(input())
set_s = set(map(int, input().split()))
number_ofcommands = int(input())

while number_ofcommands > 0:
    command_input_list = input().split()
    if command_input_list[0] == 'pop':
        set_s.pop()
    elif command_input_list[0] == 'remove':
        set_s.remove(int(command_input_list[1]))
    elif command_input_list[0] == 'discard':
        set_s.discard(int(command_input_list[1]))
    number_ofcommands -= 1 

print(sum(set_s))


```

## Set .union() Operation

```

students_englishnp = int(input())
english_roll_set = set(map(int, input().split()))
students_frenchnp = int(input())
french_roll_set = set(map(int, input().split()))

print(len(set(english_roll_set.union(french_roll_set))))


```

## Set .intersection() Operation

```

# Enter your code here. Read input from STDIN. Print output to STDOUT
students_englishnp = int(input())
english_roll_set = set(map(int, input().split()))
students_frenchnp = int(input())
french_roll_set = set(map(int, input().split()))

print(len(set(english_roll_set.intersection(french_roll_set))))

```

## Set .difference() Operation

```

# Enter your code here. Read input from STDIN. Print output to STDOUT
students_englishnp = int(input())
english_roll_set = set(map(int, input().split()))
students_frenchnp = int(input())
french_roll_set = set(map(int, input().split()))

print(len(set(english_roll_set.difference(french_roll_set))))


```

## Set .symmetric_difference() Operation

```

# Enter your code here. Read input from STDIN. Print output to STDOUT
students_englishnp = int(input())
english_roll_set = set(map(int, input().split()))
students_frenchnp = int(input())
french_roll_set = set(map(int, input().split()))

print(len(set(english_roll_set.symmetric_difference(french_roll_set))))

```

## Set Mutations

```

elements_inA = int(input())
set_A = set(map(int, input().split()))
number_of_other_setsN = int(input())

while number_of_other_setsN > 0 :
    command = list(input().split())
    space_separated_newset = set(map(int, input().split()))
    if command[0] == 'intersection_update':
        set_A.intersection_update(space_separated_newset)
    elif command[0] == 'update':
        set_A.update(space_separated_newset)
    elif command[0] == 'symmetric_difference_update' :
        set_A.symmetric_difference_update(space_separated_newset)
    elif command[0] == 'difference_update':
        set_A.difference_update(space_separated_newset)
    number_of_other_setsN -= 1

print(sum(set_A))

```

