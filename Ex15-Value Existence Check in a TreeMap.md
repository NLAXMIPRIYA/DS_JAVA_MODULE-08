# Ex15 Value Existence Check in a TreeMap

## DATE: 19-09-2026

## AIM:

To write a Java program that checks whether a given value exists in a `TreeMap` using the `containsValue()` method.

## Algorithm

1. Start and create a `TreeMap` to store key-value pairs.
2. Read the number of key-value pairs and insert them into the `TreeMap`.
3. Read the value to be searched.
4. Use the `containsValue()` method to check whether the specified value exists and display the result.
5. Stop the program.

## Program:

```java
/*
Program to check whether a given value exists in a TreeMap.
Developed by: N Laxmi Priya
RegisterNumber: 212225040196
*/

import java.util.*;

public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        TreeMap<Integer, String> map = new TreeMap<>();

        int n = sc.nextInt();

        // Read key-value pairs
        for (int i = 0; i < n; i++) {
            int key = sc.nextInt();
            String value = sc.next();
            map.put(key, value);
        }

        // Read value to search
        String searchValue = sc.next();

        // Check whether value exists
        if (map.containsValue(searchValue)) {
            System.out.println("Value exists");
        } else {
            System.out.println("Value does not exist");
        }
    }
}
```

## Output:

<img width="380" height="242" alt="image" src="https://github.com/user-attachments/assets/98deecfc-0b7e-47ff-9941-3cb84553d4fb" />


## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
