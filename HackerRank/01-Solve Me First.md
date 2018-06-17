# Problem
Complete the function solveMeFirst to compute the sum of two integers.<br> 
<b>Function prototype:</b><br>
int solveMeFirst(int x, int y);<br>
where,
<ul>
<li> x is the first integer input.</li>
<li> y is the second integer input</li>
</ul>
<b>Return values:</b>
<ul>
<li>sum of the above two integers </li>
</ul>
<b>Forrás:</b> <https://www.hackerrank.com/challenges/solve-me-first/problem> <br>
<ul>
<li>Difficulty:             Easy</li>
<li>Time Complexity:        O(1)</li>
<li>Required Knowledge:     Sum of two numbers</li>
</ul>

## C++ code

```c++
#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;

int solveMeFirst(int a, int b) {
 // Hint: Type return a+b; below:
 return a+b; 
}

int main() {
  int num1, num2;
  int sum;
  cin>>num1>>num2;
  sum = solveMeFirst(num1,num2);
  cout<<sum;
  // 1. Wait for a key press...
  //cout << << endl << endl << "Press ENTER to continue....." << endl << endl;
  //cin.ignore(1);
  //cin.ignore(1);
  
  return 0;
}
```

## Python code

```python
def solveMeFirst(a,b):
   # Hint: Type return a+b below
    return a+b
  

num1 = int(input())
num2 = int(input())
res = solveMeFirst(num1,num2)
print(res)
```

## Java code

```java
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {


    static int solveMeFirst(int a, int b) {
      	// Hint: Type return a+b; below 
        return a+b;
   }

 public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int a,b,sum;
        a = in.nextInt();
        b = in.nextInt();
        sum = solveMeFirst(a, b);
        System.out.println(sum);
   }
}
```
