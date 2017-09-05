<pre>
<h2><font color="#006699">Description</h2>
  Insertion sort works the way many people sort a hand of playing cards. 
  We start with an empty left hand and the cards face down on the table. 
We then remove one card at a time from the table and insert it into the correct 
position in the left hand. To find the correct position for a card, we compare it 
with each of the cards already in the hand, from right to left.
    Links:
        http://www.geeksforgeeks.org/insertion-sort/
        https://en.wikipedia.org/wiki/Insertion_sort
</pre>

<h2><font color="#006699">InsertionSort(_arr_)</font></h2>
<pre>
1. <b>for</b> j=2 <b>to</b> <i>arr</i>:length
2.    key = arr[<i>j</i>]
3.    <b><font color="#04B404">// Insert  <i>arr</i>[<i>j</i>] into the sorted sequence arr[<i>1..j-1<i>]</font></b>
4.    i = j-1
5.    <b>while</b> i > 0 <b>and</b> arr[i] > key
6.        <i>arr</i>[<i>i+1</i>] = <i>arr</i>[<i>i</i>]
7.        i = i-1
8.    <i>arr</i>[<i>i+1</i>] = key
</pre>

___
#### InsertionSort(arr) in Python
___
 
```python
# Python program for implementation of Insertion Sort
def insertionSort(arr):
'''
  Function to do insertion sort
  Param: arr -> Array or List
'''
  # Function to do insertion sort
  # Traverse through 1 to len(arr)
    for j in range(1, len(arr)):
        key = arr[j]
        # Move elements of arr[0..i-1], that are greater than key, 
        #to one position ahead of their current position
        i = j-1
        while i >=0 and key < arr[i] :
                arr[i+1] = arr[i]
                i -= 1
        arr[i+1] = key
 
 
# Driver code to test above
arr = [12, 11, 13, 5, 6]
insertionSort(arr)
print ("Sorted array is:")
for i in range(len(arr)):
    print ("%d" %arr[i])
 
# This code is contributed by Mohit Kumra
```
___
#### InsertionSort(arr) in Java
___
```java
// Java program for implementation of Insertion Sort
class InsertionSort
{
    /*Function to sort array using insertion sort*/
    void sort(int arr[])
    {
        int n = arr.length;
        for (int i=1; i<n; ++i)
        {
            int key = arr[i];
            int j = i-1;
 
            /* Move elements of arr[0..i-1], that are
               greater than key, to one position ahead
               of their current position */
            while (j>=0 && arr[j] > key)
            {
                arr[j+1] = arr[j];
                j = j-1;
            }
            arr[j+1] = key;
        }
    }
 
    /* A utility function to print array of size n*/
    static void printArray(int arr[])
    {
        int n = arr.length;
        for (int i=0; i<n; ++i)
            System.out.print(arr[i] + " ");
 
        System.out.println();
    }
 
    // Driver method
    public static void main(String args[])
    {        
        int arr[] = {12, 11, 13, 5, 6};
 
        InsertionSort ob = new InsertionSort();        
        ob.sort(arr);
         
        printArray(arr);
    }
} /* This code is contributed by Rajat Mishra. */
```
___
#### InsertionSort(arr) in C#/C++
___
```clike
// C program for insertion sort
#include <stdio.h>
#include <math.h>
 
/* Function to sort an array using insertion sort*/
void insertionSort(int arr[], int n)
{
   int i, key, j;
   for (i = 1; i < n; i++)
   {
       key = arr[i];
       j = i-1;
 
       /* Move elements of arr[0..i-1], that are
          greater than key, to one position ahead
          of their current position */
       while (j >= 0 && arr[j] > key)
       {
           arr[j+1] = arr[j];
           j = j-1;
       }
       arr[j+1] = key;
   }
}
 
// A utility function ot print an array of size n
void printArray(int arr[], int n)
{
   int i;
   for (i=0; i < n; i++)
       printf("%d ", arr[i]);
   printf("\n");
}
 
 
 
/* Driver program to test insertion sort */
int main()
{
    int arr[] = {12, 11, 13, 5, 6};
    int n = sizeof(arr)/sizeof(arr[0]);
 
    insertionSort(arr, n);
    printArray(arr, n);
 
    return 0;
}
```