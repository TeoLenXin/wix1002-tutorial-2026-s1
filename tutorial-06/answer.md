# Tutorial 06 - Answers
## Questions 1
### a
```java
static int max(int a, int b,int c){
    int max=a;
    
    if(b>max){
        max=b;
    }
    if(c>max){
        max=c;
    }
    
    return max;
}
    
public static void main(String[] args) {
    System.out.println(max(1, 2, 3));
}
```
### b
```java
static boolean square(int num){
    if(num<0){
        return false;
    }
    
    double root = Math.sqrt(num);
    
    if(root == Math.round(root)){
        return true;
    }else{
        return false;
    }
}
    
public static void main(String[] args) {
    System.out.println(square(9));
    System.out.println(square(10));
}
```
### c
```java
static long combination(int n, int k){
    return factorial(n) / (factorial(k) * factorial(n - k));
}

static long factorial(int num){
    long result = 1;

    for (int i=1;i<=num;i++) {
        result *= i;
    }

    return result;
}

public static void main(String[] args) {
    System.out.println(combination(3,2));
}
```
### d
```java
public static boolean pentagonal(int num) {
    if (num<1)          // the sequence starts at P1 = 1
        return false;
    
    int pentagonal = 0;
    for (int n=1;pentagonal<num;n++) {
        pentagonal = n*(3*n-1)/2;

        if (pentagonal==num){
            return true;
        }

        if (pentagonal>num){
            return false;
        }
    }
}   

public static void main(String[] args) {
    System.out.println(pentagonal(12));
    System.out.println(pentagonal(13));
}
```
### e
```java
public static void countLettersDigits(String text) {
   int letters=0;
   int digits=0;
   
   for(int i=0;i<text.length();i++){
       char ch=text.charAt(i);
       
        if (Character.isLetter(ch)){
           letters++;
        }else if (Character.isDigit(ch)){
            digits++;
        }     
    }

    System.out.println("Number of letters: " + letters);
    System.out.println("Number of digits: " + digits);
}   

public static void main(String[] args) {
    countLettersDigits("github1234");
}
```
### f
```java
public static void random(int[] num) {
   Random random = new Random();
   
    for(int i=0;i<10;i++){
        num[i]=random.nextInt(101);
        System.out.println(num[i]);
    }
}   

public static void main(String[] args) {
    int[] numbers = new int[10];
    random(numbers);
}
```
### g
```java
public static void circle(double r) {
    double area = Math.PI*r*2;
    double circumference = 2*Math.PI*r;
    
    System.out.printf("Area: %.3f\n",area);
    System.out.printf("Circumference: %.3f\n",circumference);
}

public static void main(String[] args) {
    circle(4);
}
```
### h
```java
public static int generateRandom(){
    Random rand = new Random();
    int[] arr = new int[11];
    
    while(true){
        int num = rand.nextInt(11);
        System.out.print(num+ " ");
        arr[num]++;
        if(arr[num]==2){
            return num;
        }
    }
}
public static void main(String[] args) {
    int result = generateRandom();
    System.out.println("\nFirst Repeated Number : "+result);
}
```

## Question 2
```java
public static void decresingOrder(int a , int b , int c){
    int temp;
    if(a<b){
        temp = a;
        a = b ;
        b = temp;  
    }
    
    if(a<c){
        temp = a;
        a = c ;
        c = temp;
    }
    
    if(b<c){
        temp = b;
        b = c ;
        c = temp;   
    }
    
    System.out.println(a+" "+b+" "+c);
}

public static void main(String[] args) {
    int a, b, c;
    a = 5;
    b = 15;
    c = 60;
    decresingOrder(a,b,c);
}
```
