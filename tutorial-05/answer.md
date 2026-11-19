# Tutorial 05 - Answer
## Question 1
### a
```java
float[] numbers = new float[12];
```
### b
```java
char[] value = {'A','B','C','D','E'};
```
### c
```java
String[] names = new String[100];
```
### d
```java
int[][] table = new int[6][2];
```
### e
```java
int[][] matrix = {{6,9},{2,5},{4,6}};
```
### f
```java
matrix[1][1] = 4;
matrix[2][0] = 3;
matrix[2][1] = 7;
```
### g
```java
String[] contact = {"Ali", "Abu", "Ahmad"};
        
for (int i = 0; i < contact.length; i++) {
  System.out.print((i+1)+". ");
  System.out.println(contact[i]);
}
```

## Question 2
### a
```java
String[] code = {"AAA", "AAB", "AAC", "AAD"};
```
### b
```java
int[] num = new int[10];
int sum = 0;
for(int k=0; k<num.length; k++)
  sum+=num[k];
```
### c
```java
int [][] t = new int[3][3];
t[1][2] = 5;
```
### d
```java
int i =4;
int[] score = new int[5];
score [1] = 78;
score[i] = 100;
```

## Question 3
```java
marks[0] = 961
marks[1] = 31
marks[2] = 1
marks[3] = 31
marks[4] = 31
```

## Question 4
```java
String[] sentence = {"the cat like to eat the fish in the morning"};
  
  String[] words = sentence[0].split(" ");
  
  int occurence=0;
  
  for (int i=0;i<words.length;i++){
    if(words[i].equals("the")){
        occurence++;
    }
  }
  System.out.println("The occurence of the word \"the\" is "+occurence);
}
```

## Question 5
```java
public static void main(String[] args) {
    String[] sentence = {"the cat like to eat the fish in the morning"};
    
    String[] words = sentence[0].split("");
    
    System.out.print("Reverse order: ");
    
    for(int i = words.length-1;i>=0;i--){
        System.out.print(words[i]);
    }
    System.out.println();
}
```

## Question 6
```java
import java.util.Random;
public static void main(String[] args) {
    Random random = new Random();
    
    int integer = random.nextInt(256);
    
    System.out.println("Random number: "+integer);
    
    int[] binary = new int[8];
    
    for(int i=7;i>=0;i--){
        binary[i] = integer%2;   //save binary num of index 7 first
        integer = integer/2;
    }
    
    System.out.print("Binary number: ");

    for (int i = 0; i < 8; i++) {
        System.out.print(binary[i]);  //let binary num print start from index 0
    }
    
    System.out.println();
}
```
