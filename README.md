## Adjustment for the slope m>1
Bresenham's algorithm is mainly designed for the slope 0<m<1. In this algorithm, the value of the x coordinate is increased by one unit and is checked by the decision parameter p<0 or p>=0. Based on the value of p it is decided whether to increment the y coordinate by one.

When the slope of two points becomes more than 1, it means the line is more vertical and needs to adjust to a steeper slope correctly. That's why there needs a little change which is to interchange the value of x and y.

```
#check that is steep or not
    is_steep = abs(y2 - y1) > abs(x2 - x1)

    if is_steep:
        # interchange the values
        x1, y1 = y1, x1
        x2, y2 = y2, x2
```

## Output

### Case 01 :
![image](https://github.com/SRRayhan066/Line-Drawing-Algorithm/assets/97345000/f3f1d9bf-0312-4859-803a-6d05dd46d540)

### Case 02 :
![image](https://github.com/SRRayhan066/Line-Drawing-Algorithm/assets/97345000/9c20d5ac-0ef6-4560-98a7-876558d3f2e1)
