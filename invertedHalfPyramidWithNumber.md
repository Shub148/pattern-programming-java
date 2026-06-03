# Inverted Half Pyramid with Numbers in Java

## Problem Statement

Print an inverted half pyramid pattern using numbers.

### Example Output

```text id="g7n4qx"
12345
1234
123
12
1
```

## Java Code

```java
import java.util.Scanner;
class Main{
public static void main(String[] aargs){
Scanner sc = new Scanner(System.in);
System.out.print("Enter number of rows: ");
int row = sc.nextInt();
//outer loop
for(int i = row; i>=1; i--){
//inner loop
for(int j=1; j<=i; j++){
System.out.print(j);
}
System.out.println(" ");
}
}
}
```

## Explanation

* The outer loop starts from the maximum row and decreases.
* The inner loop prints numbers from `1` to the current row number.
* After printing one row, `println()` moves to the next line.

### Working

* Row 5 → `12345`
* Row 4 → `1234`
* Row 3 → `123`
* Row 2 → `12`
* Row 1 → `1`

## Time Complexity

`O(n²)`

## Space Complexity

`O(1)`
