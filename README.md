# java-test-0002-final-13942-pranav
Final Project Assignment - This repository contains the complete final project code and documentation.


# Mirrored Number Pyramid in Java

## Problem Statement

Write a Java program to print the following mirrored number pyramid pattern using nested loops:

```
        1
      1 2 1
    1 2 3 2 1
  1 2 3 4 3 2 1
1 2 3 4 5 4 3 2 1
```

## Description

This program demonstrates how to generate a **mirrored number pyramid** using **nested loops in Java**.
The pattern increases numbers sequentially from `1` up to the current row number and then decreases back to `1`, forming a symmetric structure.

Each row contains:

* Leading spaces for alignment
* An **ascending sequence** of numbers
* A **descending sequence** of numbers

This creates a pyramid shape where the numbers mirror around the center.

## Approach

1. Define the total number of rows `n`.
2. Use an **outer loop** to iterate through each row.
3. Print **leading spaces** to center the pyramid.
4. Use a loop to print numbers in **ascending order** from `1` to the current row number.
5. Use another loop to print numbers in **descending order** from `(row-1)` back to `1`.
6. Move to the next line after each row.

## Java Implementation

```java
public class Pattern {
    public static void main(String[] args) {
        int n = 5;

        for (int i = 1; i <= n; i++) {

            for (int j = i; j < n; j++) {
                System.out.print("  ");
            }

            for (int j = 1; j <= i; j++) {
                System.out.print(j + " ");
            }

            for (int j = i - 1; j >= 1; j--) {
                System.out.print(j + " ");
            }

            System.out.println();
        }
    }
}
```

## Output

```
        1
      1 2 1
    1 2 3 2 1
  1 2 3 4 3 2 1
1 2 3 4 5 4 3 2 1
```

## Concepts Used

* Java `for` loops
* Nested loops
* Pattern printing
* Number sequencing
* Output formatting

## How to Run

1. Save the program as `Pattern.java`
2. Compile the program:

```
javac Pattern.java
```

3. Run the program:

```
java Pattern
```

## Author

Pranav Khaire
