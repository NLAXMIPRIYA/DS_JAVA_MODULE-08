# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap

## DATE: 19-09-2026

## AIM:

To implement a Java program that tracks the first unique (non-repeating) number in a stream of integers using a `LinkedHashMap`.

## Algorithm

1. Start and create a `LinkedHashMap` to store each integer and its frequency of occurrence.
2. Read the number of elements and insert each integer into the `LinkedHashMap`, updating its frequency.
3. Traverse the `LinkedHashMap` in insertion order.
4. Find and display the first number whose frequency is `1`; if no such number exists, display `-1`.
5. Stop the program.

## Program:

```java
/*
Program to track the first unique (non-repeating) number
in a stream of integers using a LinkedHashMap.
Developed by: N Laxmi Priya
RegisterNumber: 212225040196
*/

import java.util.*;

public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        LinkedHashMap<Integer, Integer> map = new LinkedHashMap<>();

        int n = sc.nextInt();

        // Read stream elements and update frequency
        for (int i = 0; i < n; i++) {

            int num = sc.nextInt();

            map.put(num, map.getOrDefault(num, 0) + 1);

            // Find the first unique number
            int firstUnique = -1;

            for (int key : map.keySet()) {
                if (map.get(key) == 1) {
                    firstUnique = key;
                    break;
                }
            }

            System.out.println(firstUnique);
        }
    }
}
```

## Output:

<img width="377" height="249" alt="image" src="https://github.com/user-attachments/assets/d93e71ad-290d-48fe-b4bc-5c435c9fbb3e" />



## Result:
The program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
