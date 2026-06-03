# Inverted Rotated Half Pyramid (Rotated by 180 Degree) in Java

## Problem Statement

Print an inverted rotated half pyramid pattern (rotated by 180°) using `*`.

### Example Output

```text id="w72nfa"
    *
   **
  ***
 ****
*****
```

## Java Code

```java
     import java.util.Scanner;
class file Name{
public static void main(String[] args){
Scanner sc = new Scanner(System.in);
int row = sc.nextInt();
System.out.print("Enter number of rows: ");
//for outer loop
for(int i=1; i<=row; i++){
//inner loop- used to  print space
for(int j=1; j<=row-i; j++){
System.out.print(" ");
}
// inner loop - to print star
for(int j=1; j<=i; j++){
System.out.print("*");
}
System.out.println();
}

}
```

## Explanation

* The outer loop controls the number of rows.
* The first inner loop prints spaces to shift stars to the right.
* The second inner loop prints `*` according to the row number.
* Together, this creates a half pyramid rotated by 180°.

### Working

* Row 1 → `    *`
* Row 2 → `   **`
* Row 3 → `  ***`
* Row 4 → ` ****`
* Row 5 → `*****`

## Time Complexity

`O(n²)`

## Space Complexity

`O(1)`
