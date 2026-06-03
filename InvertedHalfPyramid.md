# Inverted Half Pyramid Pattern in Java

## Problem Statement

Print an inverted half pyramid pattern using `*`.

### Example Output

```text id="xv82p1"
*****
****
***
**
*
```

## Java Code

```java
import java.util.Scanner;
class file name{
public static void main(String[] args){
System.out.print("Enter number of rows: ");
int row = sc.nextInt();
for(int i=row; i>=1; i--){
for(int j=1; j<=i; j++){
System.out.print("*");
}
System.out.println();
}
}
}
```

## Explanation

* The outer loop starts from the maximum number of rows and decreases.
* The inner loop prints `*` according to the current row number.
* After printing stars in one row, `println()` moves to the next line.

### Working

* Row 5 → `*****`
* Row 4 → `****`
* Row 3 → `***`
* Row 2 → `**`
* Row 1 → `*`

## Time Complexity

`O(n²)`

## Space Complexity

`O(1)`
