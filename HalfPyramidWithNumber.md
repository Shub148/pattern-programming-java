# Half Pyramid with Numbers in Java

## Problem Statement

Print a half pyramid pattern using numbers.

### Example Output

```text id="r8m2vz"
1
12
123
1234
12345
```

## Java Code

```java
import java.util.Scanner;
class file name{
public static void main(String[] args){
Scanner sc =new Scanner(System.in);
System.out.print("Enter number of rows: ");
int row = sc.nextInt();
//outer loop
for(int i=1; i<=row; i++){
//inner loop
for(int j=1; j<=i; j++){
//print number so that is why used j
System.out.print(j);
}
System.out.println();

}

}


}


```

## Explanation

* The outer loop controls the number of rows.
* The inner loop prints numbers from `1` to the current row number.
* After printing one row, `println()` moves to the next line.

### Working

* Row 1 → `1`
* Row 2 → `12`
* Row 3 → `123`
* Row 4 → `1234`
* Row 5 → `12345`

## Time Complexity

`O(n²)`

## Space Complexity

`O(1)`
