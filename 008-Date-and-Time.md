# Date and Time

## Calendar Module 

```

import calendar

date_input_list = list(map(int, input().split()))
weekday_ = calendar.weekday(date_input_list[2], date_input_list[0], date_input_list[1])

if weekday_ == 0:
    print('MONDAY')
elif weekday_ == 1:
    print('TUESDAY')
elif weekday_ == 2:
    print('WEDNESDAY')
elif weekday_ == 3:
    print('THURSDAY')
elif weekday_ == 4:
    print('FRIDAY')
elif weekday_ == 5:
    print('SATURDAY')
elif weekday_ == 6:
    print('SUNDAY')

```

## Time Delta

```

- [ ] #todo

```
