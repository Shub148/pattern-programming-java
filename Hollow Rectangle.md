# Hollow Rectangle Pattern

## Problem Statement

Print a hollow rectangle pattern using stars (`*`) for the given number of rows and columns.

### Example Input

```
Rows = 4
Columns = 5
```

### Output

```
*****
*   *
*   *
*****
```

## Approach

* Print `*` on the first and last rows.
* Print `*` on the first and last columns.
* Print spaces in all other positions.

## Java Code

```java

import java.util.Scanner;
class file name{
public static void main (String[] args){
Scanner sc = new Scanner(System.in);
System.out.println("Enter number of rows");
int row = sc.nextInt();
System.out.println("Enter number of Columns");
int col = sc.nextInt();
for(int i=1; i<=row; i++){
for(int j=1; j<=col; j++){
if(i==1 || j==1 || i==row || j==col){
System.out.print("*");
}else{
System.out.print(" ");
}
}
System.out.println("");
}
}
}
```

## Dry Run

For `Rows = 4` and `Columns = 5`:

* Row 1 → Print all stars
* Row 2 → Print star at beginning and end
* Row 3 → Print star at beginning and end
* Row 4 → Print all stars

## Time Complexity

**O(rows × columns)**

## Space Complexity

**O(1)**

## Concepts Used

* Nested Loops
* Conditional Statements (`if-else`)
* Pattern Printing
