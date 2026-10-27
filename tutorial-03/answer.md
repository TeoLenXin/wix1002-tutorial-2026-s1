# Tutorial 03 - Answers

## Question 1
### a
```java
public static void main(String[] args) {
  if (3*8==27){
    System.out.println("True");
  }else{
    System.out.println("False");
  }
}

//boolean isEqual = 3*8 ==27;
//System.out.println(isEqual);
```
### b
```java
import java.util.Scanner;

public static void main(String[] args) {
  Scanner input = new Scanner(System.in);
        
  System.out.print("Enter an integer: ");
  int num = input.nextInt();
        
  if (num%2 == 0){
    System.out.println("Even number");
  }else{
    System.out.println("Odd number");
  }
}
```
### c
```java
public static void main(String[] args) {
  char character = 'A';
        
  if (character>='A' && character <='Z'){             //because ASCII table
    System.out.println("It is a capital letter.");
  }else{
    System.out.println("It is not a capital letter.");
  }
}
```
### d
```java
public static void main(String[] args) {
  String first = "Good";
  String second = "Question";
        
  if (first.compareToIgnoreCase(second)<0){        // < ascending, > descending
    System.out.println(first);
    System.out.println(second);
  }else{
    System.out.println(second);
    System.out.println(first); 
  }
}
```
### e
```java
import java.util.Scanner;

public static void main(String[] args) {
  Scanner input = new Scanner(System.in);

  System.out.print("Enter number 0-6: ");
  int day = input.nextInt();
          
  switch(day){
    case 0:
      System.out.println("Sunday");
      break;
    case 1:
      System.out.println("Monday");
      break;
    case 2:
      System.out.println("Tuesday");
      break;
    case 3:
      System.out.println("Wednesday");
      break;
    case 4:
      System.out.println("Thursday");
      break;
    case 5:
      System.out.println("Friday");
      break;
    case 6:
      System.out.println("Saturday");
      break;
    default:
      System.out.println("Invalid input");
  }
}
```

## Question 2
### a
```java
if (num1 == num2)
  System.out.println("Number 1 is equal to number 2.");
```
### b
```java
if (x > y  &&  x > z)
  System.out.println("x is the largest number");
```
### c
```java
String s1, s2;
if (s1.equals(s2))        //compare between two string
  System.out.println("They are equal strings."); 
else 
  System.out.println("They are not equal strings.");
```
### d
```java
if (x>0 || y>0)
  System.out.println("Either x or y is positive");
```

## Question 3
### a
```
#####
$$$$$
```
### b
```
#####
$$$$$
```
### c
```
#####
```
### d
```
No output
```

## Question 4
```java
public static void main(String[] args) {
  int num1 = 1;
  int num2 = 2;
  int num3 = 3;
        
  if (num1>=num2 && num1>=num3){
    System.out.println("Biggest number is "+num1);
  }else if(num2>=num1 && num2>=num3){
    System.out.println("Biggest number is "+num2);
  }else{
    System.out.println("Biggest number is "+num3);
  }     
}
```

## Question 5
```java
public static void main(String[] args) {
  int year = 2026;
        
  if ((year%4 == 0 && year%100 != 0) || year%400 == 0){
    System.out.println(year+" is a leap year.");
  }else{
    System.out.println(year+" is not a leap year.");
  }        
}
```
