public class Patterns{
    public static void printHelloWorld(){
        System.out.println("Hello World");
        System.out.println("Hello World");
        System.out.println("Hello World");
    }
    public static void main(String args[]){
        printHelloWorld();
    }
}


# 2. Argumensts & Parameters

import java.util.*;
public class Patterns{
    public static void printHelloWorld(){
        System.out.println("Hello World");
        System.out.println("Hello World");
        System.out.println("Hello World");
    }
    public static int calculateSum(int  a, int b){ //parameters
        int sum = a+b;
        return sum;
        
    }
    public static void main(String args[]){ 
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        int sum = calculateSum(a,b); //arguments
        System.out.println("Sum is: "+ sum);
    }
}

# 3. Factorial 

import java.util.*;
public class Patterns{

    public static int factorial(int n){
        int f=1;
        for(int i=1; i<=n; i++){
            f = f*i;
        }
        return f;
    }

    public static void main(String args[]){ 
        System.out.println(factorial(4));
    }
}

# Float

import java.util.*;
public class Patterns{
    public static float sum(float a , float b){
        return a+b;
    }

    public static void main(String args[]){ 
        System.out.println(sum(3,5));
    }
}

# is prime

    public static boolean isPrime(int n){
        boolean isPrime = true;

        if(n==2){
            return true;
        }
        for(int i=2; i<=n-1; i++){
            if(n%i==0){
                isPrime = false;
                break;
            }
        }
        return isPrime;
    }

    public static void main(String args[]){ 
        System.out.println(isPrime(8));
    }
}

# more optimized wayfor is Prime

    public static boolean isPrime(int n){
        if(n==2){
            return true;
        }

        for(int i=2; i<=Math.sqrt(n); i++){
            if(n % i == 0){
                return false;
            }
        }
        return true;
    }

    

    public static void main(String args[]){ 
        System.out.println(isPrime(17));
    }
}

# print all primes in a range

import java.util.*;
public class Patterns{

    public static boolean isPrime(int n){
        if(n==2){
            return true;
        }

        for(int i=2; i<=Math.sqrt(n); i++){
            if(n % i == 0){
                return false;
            }
        }
        return true;
    }

    public static void primeInRange(int n){
        for(int i=2; i<=n; i++){
            if(isPrime(i)){
                System.out.print(i+" ");
            }
        }
        System.out.println();
    }
    public static void main(String args[]){ 
        primeInRange(50);
    }
}

# Convert from Binary to decimal

import java.util.*;
public class Patterns{

    public static void binToDec(int binNum){
        int pow =0;
        int decNum = 0;

        while(binNum > 0){
            int lastDigit = binNum % 10;
            decNum = decNum + (lastDigit * (int)Math.pow(2,pow));

            pow++;
            binNum = binNum/10;
        }
        System.out.println("decimal of" + binNum + "=" + decNum);
    }

    public static void main(String args[]){ 
        binToDec(101);
    }
}