# Ex12 Add Elements from an Array into a TreeSet

## DATE: 19-09-2026

## AIM:

To write a Java program that adds elements from an array into a `TreeSet` and displays the elements in sorted order.

## Algorithm

1. Start and read the number of elements and initialize an integer array.
2. Read the elements into the array.
3. Create a `TreeSet` and add all the array elements using a loop.
4. Traverse the `TreeSet` and display the elements in sorted order.
5. Stop the program.

## Program:

```java
/*
Program that adds elements from an array into a TreeSet and
displays the elements in sorted order.
Developed by: N Laxmi Priya
RegisterNumber: 212225040196
*/

import java.util.*;

public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        int[] arr = new int[n];

        // Read array elements
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        // Create TreeSet
        TreeSet<Integer> set = new TreeSet<>();

        // Add array elements to TreeSet
        for (int i = 0; i < n; i++) {
            set.add(arr[i]);
        }

        // Display elements in sorted order
        System.out.println("TreeSet: " + set);
    }
}
```

## Output:

<img width="382" height="173" alt="image" src="https://github.com/user-attachments/assets/76c379bb-5ad3-4111-811e-a38adc48e1ca" />



## Result:
The program successfully adds elements from an array into a TreeSet.
