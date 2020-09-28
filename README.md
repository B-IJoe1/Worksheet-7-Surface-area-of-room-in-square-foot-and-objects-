package lab02;
import java.util.Scanner;

public class HelloWorld
{


     public static void main (String[] args)
    {

    	 
    //Length, width, and height of the room in feet	 
    	 
    	Scanner input = new Scanner (System.in);
    	
   System.out.println("Enter the length of the room in feet");
   
   double length = input.nextDouble();
   
   
   System.out.println("Enter the width of the room in feet");
   
   double width = input.nextDouble();
   
   
   System.out.println("Enter the height of the room in feet");
   
   double height = input.nextDouble();
   
   
   
   
 
   
   
   
   //Surface area of the walls in square feet
   
   System.out.println("Calculate the surface area of the room in square feet" );
   
   double surfacearea = (length + width + length + width)  * height;
   
   System.out.println("(length + width + length + width) * height = " + surfacearea + " " + "square feet" );
   
    
   
   
   
   
   
   
   //Length and width of the door in square feet
    	
   	System.out.println("Enter the width of the door in feet");
   	
   	double width1 = input.nextDouble();
   	
   	
   	System.out.println("Enter the length of the door in feet");
   	
   	double length1 = input.nextDouble();
   	
   	double result1 = length1 * width1;
   	
   	System.out.println("length1 * width1 = " + result1 + " " + "square feet");
   	
   	
   	
   	
   	
   	
   	
   	
   	//The width and length of the windows in square feet
   	
   	System.out.println("Enter the width of the windows in feet");
   	
   	double width2 = input.nextDouble();
   	
   	System.out.println("Enter the length of the windows in feet");
   	
   	double length2 = input.nextDouble();
   	
   	double result2 = length2 * width2 * 2;
   	
   	System.out.println ("length2 * width2 * 2 = " + result2 + " " + "square feet");
   	
   	
   	
   	
   	
   	
   	
   	
  //The length and width of the window in square feet  	
   	
System.out.println("Enter the width of the bookshelf in feet");
   	
   	double width3 = input.nextDouble();
   	
   	System.out.println("Enter the length of the bookshelf in feet");
   	
   	double length3 = input.nextDouble();
   	
   	double result3 = length3 * width3;
   	
   	System.out.println("length3 * width3 = " + result3 + " " + "square feet");
   	
   	
   	
   	
   	
   	
   	
   	//The surface area of the wall
   	
   	System.out.println("Surface area of the wall = Surface area of room - area of door - area of windows - area of bookshelf =" );
   	
   	double result4 = surfacearea - result1 - result2- result3;
   	
   	System.out.println(result4);
   	
   	
   	
   	
   	
   	
   	
   	
   	//User input: The cost of paint per square foot
   	
   	System.out.println("Enter the cost of the paint you want to purchase per square foot");
   	
   	double paintcost = input.nextDouble();
   	
   	double result5 = result4 * paintcost;
   	
   	System.out.println("Cost of paint per square foot * surface area of the wall = " + result5 + " " + "dollars" );
   	
   	
   	
   	

   	
   	
   	
   	//User input: The cost of the carpet per square foot
   	
   	System.out.println("Enter the cost of the carpet you want to purchase per square foot");
   	
   	double carpetcost = input.nextDouble();
   	
   	double result6 = carpetcost * (length * width);
   	
   	System.out.println("Carpet cost per square foot = " + result6 + " " + "dollars");
   	
   	
   	
   	
   
   	
   	
   	
   	//Total cost of installing the carpet and painting the walls
   	
   	System.out.println("Cost of painting the wall and installing the carpet");
   	
   	
   	double result7 = result5 + result6;
   	
   	System.out.println(result7 + " " + "dollars");

input.close();


} }
