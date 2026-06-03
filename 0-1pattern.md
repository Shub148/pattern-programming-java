# 0-1 Pattern in Java

## Problem Statement

Print a 0-1 pattern using numbers.

### Example Output

```text id="k3v9pn"
1
0 1
1 0 1
0 1 0 1
1 0 1 0 1
```

## Java Code

```java
import java.util.Scanner;
class Main{
public static void main(String[] args){
Scanner sc = new Scanner(System.in);
int row = sc.nextInt();
for(int i=1; i<=row; i++){
for(int j=1; j<=i; j++){ 
int sum = i+j;
if(sum%2==0){
System.out.print("1");
}else{
System.out.print("0");
}
}
System.out.println();
}
}
}
```

## Explanation

* The outer loop controls the number of rows.
* The inner loop prints values for each column.
* If `(row + column)` is even, print `1`.
* If `(row + column)` is odd, print `0`.
* `println()` moves to the next line after each row.

### Working

* Row 1 → `1`
* Row 2 → `0 1`
* Row 3 → `1 0 1`
* Row 4 → `0 1 0 1`
* Row 5 → `1 0 1 0 1`

## Time Complexity

`O(n²)`

## Space Complexity

`O(1)`
