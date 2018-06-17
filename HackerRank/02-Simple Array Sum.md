# Simple Array Sum

# Problem
Given an array of integers, find the sum of its elements.<br>
<b>Input Format</b><br>
The first line contains an integer, , denoting the size of the array.<br>
The second line contains space-separated integers representing the array's elements.<br>
<b>Output Format:</b><br>
Print the sum of the array's elements as a single integer.<br>
<b>Sample Input:</b><br>
6<br>
1 2 3 4 10 11<br>
<br>
<b>Sample Output:<b><br>
31<br>
<br>
<b>Forrás:</b> <https://www.hackerrank.com/challenges/simple-array-sum/problem> <br>
<ul>
<li>Difficulty:             Easy</li>
<li>Time Complexity:        O(n)</li>
<li>Required Knowledge:     for loops</li>
</ul>

## C++ code

```c++
#include <math.h>
#include <stdio.h>
#include <string.h>
#include <stdlib.h>
#include <assert.h>
#include <limits.h>
#include <stdbool.h>

int main(){
    int n; 
    scanf("%d",&n);
    int arr[n]; int sum=0;
    for(int arr_i = 0; arr_i < n; arr_i++){
       scanf("%d",&arr[arr_i]); sum+=arr[arr_i];
    }
    printf("%d",sum);
    return 0;
}
```

## Python code

```python
#!/bin/python3
import sys

n = int(input().strip())
arr = [int(arr_temp) for arr_temp in input().strip().split(' ')]
print(sum(arr))
```

## Java code

```java
```
