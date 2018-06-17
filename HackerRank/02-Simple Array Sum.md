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
import java.io.*;
import java.math.*;
import java.text.*;
import java.util.*;
import java.util.regex.*;

public class Solution {

    /*
     * Complete the simpleArraySum function below.
     */
    static int simpleArraySum(int[] ar) {
        int sumOfArray = 0;
        for(int i = 0; i < ar.length; i++) {
            sumOfArray += ar[i];
        }
        return  sumOfArray;
    }

    private static final Scanner scanner = new Scanner(System.in);

    public static void main(String[] args) throws IOException {
        BufferedWriter bufferedWriter = new BufferedWriter(new FileWriter(System.getenv("OUTPUT_PATH")));

        int arCount = Integer.parseInt(scanner.nextLine().trim());

        int[] ar = new int[arCount];

        String[] arItems = scanner.nextLine().split(" ");

        for (int arItr = 0; arItr < arCount; arItr++) {
            int arItem = Integer.parseInt(arItems[arItr].trim());
            ar[arItr] = arItem;
        }

        int result = simpleArraySum(ar);

        bufferedWriter.write(String.valueOf(result));
        bufferedWriter.newLine();

        bufferedWriter.close();
    }
}
```
