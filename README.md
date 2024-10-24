Printing Rhombus Star Pattern
In this JAVA program we will be coding a rhombus star pattern which will have n number of stars in it rows and n of stars in column hence it will be a n x n rhombus star pattern  
Print Rhombus Star Pattern
Printing Pattern
In this JAVA program we will be coding a rhombus star pattern which will have n number of stars in it rows and n of stars in column hence it will be a n x n rhombus star pattern

Prerequisite:
Basic knowledge of Java language and loops

Algorithm:
Take the number of rows as input from the user and store it in any variable.(‘row‘ in this case).
Take the number of coloum as input from the user and store it in any variable.(‘col‘ in this case).
Run a loop ‘row’ number of times to iterate through each of the rows. From i=1 to i<=row. The loop should be structured as for                                     (int i=1; i<= row; i++)
 Run a nested loop inside the main loop to print the spaces before the rhombus. From j=1 to j<=i. The loop should be structured as for( j=1; j<=i ; j++).
Run another nested loop inside the main loop after the previous loop to print the stars in each column of a row. From j=1 to j<=col. The loop should be structured as for( j=1 ; j<=col ; j++).
Move to the next line by printing a new line . System.out.print(“*”);
After that take System.out.println(); at the end of main for loop
Code in Java:
import java.util.Scanner;
public class Pattern1 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.println("Enter row and col");
		int row = sc.nextInt();
		int col = sc.nextInt();
		
		for (int i=1; i<= row; i++) {
			for (int j=1 ; j<=i ; j++)  // this loop is for printing spaces
				System.out.print(" ");
			for (int j=1 ; j<=col; j++) // this loop is for printing stars
				System.out.print("*");
			System.out.println();
		}

	}

}

