# Solid Rectangle Pattern

## Problem Statement

Print a solid rectangle pattern of stars (`*`) for the given number of rows and columns.

### Example Input

```
Rows = 4
Columns = 5
```

### Output

```
*****
*****
*****
*****
```

## Approach

* Use an outer loop to iterate through rows.
* Use an inner loop to print stars for each column.
* After printing one row, move to the next line.

## Java Code

```java
import java.util.Scanner;

public class SolidRectangle {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Enter number of rows: ");
        int rows = sc.nextInt();  // Take input from user of row

        System.out.println("Enter number of columns: ");
        int cols = sc.nextInt();  // Take input from user of column

        for (int i = 1; i <= rows; i++) {  // for row condition

            for (int j = 1; j <= cols; j++) {  // for column condition
                System.out.print("*");//not used println because it print on next line but we want it must present on same line that is why we used print so it //print till it satisfy the condition
            }

            System.out.println(); // Move to next line
        }

        
    }
}
```

## Time Complexity

* **O(rows × columns)**

## Space Complexity

* **O(1)**
