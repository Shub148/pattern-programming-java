# Half Pyramid Pattern in Java

## Problem Statement

Print a half pyramid pattern using `*`.

### Example Output

```text
*
**
***
****
*****
```

## Java Code

```java
import java.util.Scanner;
class file name{
public class static void main(String[] args){
Scanner sc = new Scanner(System.in);
System.out.println("Enter number of rows:");
int row = sc.nextInt();  // take input from the user for row

for(i=1; i<=row; i++){
for(j=1; j<=i; j++){   // Here as a number of row same as a number of columns that is why we intitialised the row with 1 but less than and equal to i or row
System.out.print("*");
}
System.out.println(); // Moed to next line 
}


}

}
```

## Explanation

* The outer loop controls the number of rows.
* The inner loop prints `*` according to the current row number.
* After printing stars in one row, `println()` moves to the next line.

### Working

* Row 1 → `*`
* Row 2 → `**`
* Row 3 → `***`
* Row 4 → `****`
* Row 5 → `*****`

## Time Complexity

`O(n²)`

## Space Complexity

`O(1)`
