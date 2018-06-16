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
  return 0;
}
```
