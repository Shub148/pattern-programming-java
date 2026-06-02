# pattern-programming-java
This contains pattern programming question.
1) SOLID RECTANGLE

   import java.util.Scanner;
   class file name{
   public class static void main(String[] args){
Scanner sc = new Scanner(System.in);
System.out.println("Enter number of rows");
int row = sc.nextInt();  // take input of row from user
System.out.println("Enter number of columns");
int col = sc.nextInt();  // take input of column from user
for(int i = 1; i<=row; i++){  // for row condition
for(int j = 1; j<=col; j++){  // for column condition
System.out.print("*");  //not used println because it print on next line but we want it must present on same line that is why we used print so it print till it //satisfy the condition
}
System.out.println();// Moved to next line
}


   }
   }
