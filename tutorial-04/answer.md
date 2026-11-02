# Tutorial 04 - Answers
## Question 1
### a
```java
public static void main(String[] args) {
  int n = 0;
        
  while ((n + 1) * (n + 1) * (n + 1) < 2000) {
    n++;
  }
  System.out.println("n = " + n);
}
```
### b
```java
public static void main(String[] args) {
  int num = 1;
        
  while (num < 13){
    int square = num*num;
    System.out.println("Square number of "+num+" is "+square);
    num++;
  }
}
```
### c
```java
import java.util.Random;
public static void main(String[] args) {
  Random random = new Random();
        
  for (int row = 1; row <= 4; row++){
    for (int col = 1; col <= 5; col++) {
      int num = random.nextInt(101);
      System.out.print(num+" ");
    }
    System.out.println();
  }
}
```
### d
```java
import java.util.Scanner;
public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        
        System.out.print("Enter a number: ");
        int num = input.nextInt();
        
        int sum=0;
        
        for(int i=1;i<=num;i++){
            sum = sum + i;
        }
        System.out.println("Sum of 1 to " + num + " = " + sum);
}
```
### e
```java
public static void main(String[] args) {
        double sum=0;
        
        for(double i=1;i<=25;i++){
            sum += i / (26 - i);
        }
        System.out.printf("Sum of the series is %.2f%n",sum);    
}
```

## Question 2
### a
```java
int sum = 0;
for (int x = 10; x > 0; x--)
  sum += x;
```
### b
```java
int x = 0, y = 0;
do{
  x += 2;
  y += x;
  System.out.println(x + " and " + y);
}while (x < 100);
```
### c
```java
int x, y;
  for ( x=1, y=20; x < y, x++, y-=2);
  System.out.println(x + " " + y);
```
### d
```java
int i = 1;
while (i <= 10) {
    if (i == 10)
       	System.out.println("Program End");
    i++;
}
```

## Question 3
```java
public static void main(String[] args) {
        int previous=1;
        int current=1;
        int next;
        
        System.out.print(previous+" "+current);
        
        for (int num=3;num<=10;num++){
            next = previous + current;
            System.out.print(" "+next);
            previous = current; 
            current = next;
        }
         System.out.println();    
}
```

## Question 4
```java
import java.util.Scanner;
public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter a string: ");
        String letter = input.nextLine();
        
        System.out.print("Reverse string: ");

        for (int i = letter.length()-1; i>=0; i--) {
            System.out.print(letter.charAt(i));
        } 
}
```
