# Ex11 Convert HashSet to ArrayList in Java

## DATE: 19-09-2026

## AIM:

To convert a collection of distinct integers stored in a `HashSet` into an `ArrayList` and display its contents.

## Algorithm

1. Start and create a `HashSet` to store distinct integer elements.
2. Add the given integers to the `HashSet`.
3. Create an `ArrayList` by passing the `HashSet` to its constructor.
4. Traverse the `ArrayList` and display its elements.
5. Stop the program.

## Program:

```java
/*
Program to convert a collection of distinct integers stored in a
HashSet into an ArrayList and display its contents.
Developed by: N Laxmi Priya
RegisterNumber: 212225040196
*/

import java.util.*;

public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        HashSet<Integer> set = new HashSet<>();

        int n = sc.nextInt();

        // Read elements into HashSet
        for (int i = 0; i < n; i++) {
            set.add(sc.nextInt());
        }

        // Convert HashSet to ArrayList
        ArrayList<Integer> list = new ArrayList<>(set);

        // Display ArrayList
        System.out.println("ArrayList: " + list);
    }
}
```

## Output:

<img width="372" height="176" alt="image" src="https://github.com/user-attachments/assets/d9992146-eeff-4c99-8282-c3d52188532a" />



## Result:
The program successfully converts a collection of distinct integers stored in a HashSet into an ArrayList
