# Tutorial 02 - Answers

## Question 1
### a.
System.out.print("Faculty of  ");
System.out.print("Computer Science ");
System.out.println("and Information Technology");
### b.
System.out.println("Faculty of \nComputer Science \nand Information Technology");

## Question 2
System.out.println("\"SDN\" - Software-defined networking");

## Question 3
### a.
System.out.println("Java Programming");
### b.
System.out.println("Introduction to Java!");
### c.
System.out.println("\\t is the horizontal tab character");
### d.
System.out.println("Java is case sensitive!" ); 

## Question 4
### a.
String matricnumber;
### b.
double pi;
### c.
boolean M = false; 
### d.
long P = 8800000000;
### e.
char letter = ‘U’
### f.
final String PRO = “Java”;

## Question 5
### a.
double AMOUNT = 32.5; 
AMOUNT += 10; 
System.out.println("The amount is " + AMOUNT); 
### b.
String chapter = “Summary”; 
System.out.println(chapter); 
### c.
int num = 0;
num++;
int num1 = num;
### d.
double num = 3000;
System.out.printf("%4.2f\n", num);
### e.
String contact;
Scanner keyboard = new Scanner(System.in);
contact = keyboard.nextLine();

## Question 6
```java
import java.util.Scanner;

public class Q6 {

    public static void main(String[ ] args) {
       Scanner input = new Scanner(System.in);
       
       double diameter;
       double circumference;
       
       System.out.print("Enter diameter: ");
       diameter = input.nextDouble();
       
       circumference = Math.PI*diameter;
       
        System.out.printf("The circumference of the circle is: %.3f\n",circumference);
       
    }
    
}
```

## Question 7
```java
import java.util.Scanner;

public class Q7 {

    public static void main(String[ ] args) {
       Scanner input = new Scanner(System.in);
       
       double inch;
       double meter;
       
       System.out.print("Enter value in inch: ");
       inch = input.nextDouble();
       
       meter = inch*0.0254;
       
        System.out.printf("%.2f inches = %.2f meters\n",inch,meter);
        
    }
    
}
```
