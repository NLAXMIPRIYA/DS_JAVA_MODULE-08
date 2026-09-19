# Ex13 Fill the First 10 Elements of an Array with a Constant using Arrays.fill()

## DATE: 19-09-2026

## AIM:

To write a Java program that fills the first 10 elements of an array with a constant value using the `Arrays.fill()` method.

## Algorithm

1. Start and create an integer array with at least 10 elements.
2. Initialize the array with default values.
3. Use `Arrays.fill()` to fill the first 10 elements with the constant value `5`.
4. Display the array elements using a loop.
5. Stop the program.

## Program:

```java
/*
Program to fill the first 10 elements of an array with a
constant value using the Arrays.fill() method.
Developed by: N Laxmi Priya
RegisterNumber: 212225040196
*/

import java.util.Arrays;

public class Main {

    public static void main(String[] args) {

        int[] arr = new int[15];

        // Fill the first 10 elements with 5
        Arrays.fill(arr, 0, 10, 5);

        // Display the array
        System.out.println("Array elements:");

        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i] + " ");
        }
    }
}
```

## Output:

<img width="371" height="194" alt="image" src="https://github.com/user-attachments/assets/ed72f1dd-dd8a-4020-923e-83e92fc8c7e8" />


## Result:
The program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
