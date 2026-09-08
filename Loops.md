# Counter to print a large number of data 

public class JavaBasics{
    public static void main (String args[]){
        int counter = 0;
        while(counter<100){
            System.out.println("Hello World");
            counter++;
        }
     }
 }

# print numbers


public class JavaBasics{
    public static void main (String args[]){
        int counter =1;
        while(counter <= 10){
            System.out.print(counter + " ");
            counter++;
        }
        System.out.println();
        }
    }

# do-while Loop


public class JavaBasics{
    public static void main (String args[]){
        int counter =1;
        do { 
            System.out.println("Hello World");
            counter++;
        } while (counter <= 10);
        }
    }

# Reverse of a number


public class JavaBasics{
    public static void main (String args[]){
        int n = 10899;
        while(n>0){
            int lastDigit = n %10;
            System.out.println(lastDigit);
            n=n/10;
        }
        }
    }

# Display all numbers entered by user except multiples of 10

import java.util.Scanner;

public class JavaBasics{
    public static void main (String args[]){
       Scanner sc = new Scanner(System.in);
       do { 
           System.out.print("Enter Your Number: ");
           int n = sc.nextInt();

           if(n%10 == 0){
            continue;
           }
           System.out.println("Number was: " + n);
       } while (true);
        }
    }

# KEep entering numbers till user enters a multiple of 10

