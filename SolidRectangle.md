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

        System.out.print("Enter number of rows: ");
        int rows = sc.nextInt();

        System.out.print("Enter number of columns: ");
        int cols = sc.nextInt();

        for (int i = 1; i <= rows; i++) {

            for (int j = 1; j <= cols; j++) {
                System.out.print("*");
            }

            System.out.println();
        }

        
    }
}
```

## Time Complexity

* **O(rows × columns)**

## Space Complexity

* **O(1)**
