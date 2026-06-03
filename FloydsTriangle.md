# Floyd's Triangle in Java

## Problem Statement

Print Floyd’s Triangle pattern using numbers.

### Example Output

```text id="n8v2pk"
1
2 3
4 5 6
7 8 9 10
11 12 13 14 15
```

## Java Code

```java
import java.util.Scanner;
class file name{
public static void main(String[] args){
Scanner sc = new Scanner(System.in);
int row = sc.nextInt();
int number = 1;
for(int i=1; i<=row; i++){
for(int j=1; j<=i; j++){ 
System.out.print(number);
number++;
}
System.out.println();
}
}
}
```

## Explanation

* The outer loop controls the number of rows.
* A variable `number` starts from `1`.
* The inner loop prints the number and increments it after every print.
* `println()` moves to the next line after each row.

### Working

* Row 1 → `1`
* Row 2 → `2 3`
* Row 3 → `4 5 6`
* Row 4 → `7 8 9 10`
* Row 5 → `11 12 13 14 15`

## Time Complexity

`O(n²)`

## Space Complexity

`O(1)`
