Calculator-Final
================

// By Reina Olarte

import java.util.Scanner;
// Imports the scanner class

public class Calculator 

{

	// Execution of JAva Program  Main Method begins:
	
public static void main( String[]args )
{
	
	//  Input information  ( Create a scanner)
	
	Scanner input = new Scanner(System.in);
	
	// Declaring the variables
	
	int Number1;
	int Number2;
	int Output;
	
	String operation;
	
	System.out.println("Enter the First digit: ");
	
	Number1 = input.nextInt();
	
	System.out.println("Enter the Second Digit: ");
	
	Number2 = input.nextInt();
	
	System.out.println("Please enter the operation : \n (+  ,  -  ,  *  ,  /  , %  )");
	
	
	operation = input.next();
	
	if (operation.equals( "+"))
	{
		Output= Number1 + Number2;
		System.out.printf("The  Addition of %d + %d = %d\n", Number1, Number2, Output);
			
	}
	else if (operation.equals( "-"))
	{
		Output= Number1 - Number2;
		System.out.printf("The subtraction of %d - %d  =\n", Number1, Number2, Output);
	}
	else if (operation.equals ( "/"))
	{
		Output= Number1 / Number2;
		System.out.printf("The Division of %d / %d = %d\n ", Number1, Number2, Output);
	}
	else if (operation.equals( "*"))
			{
		Output= Number1 * Number2;
		System.out.printf( "The multiplication of %d X %d = %d\n", Number1, Number2, Output);
			}
	
	else if (operation.equals( "%"))
	{		
	
		Output= Number1 % Number2;
		System.out.printf("The Remainder of %d Mod %d = %d\n", Number1, Number2,Output);
		
	}
	
	else 
		System.out.println("Wrong entered");
	
}  // End method main
	
}  // End class
