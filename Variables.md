public class JavaBasics{
    public static void main(String args[]){
        char a = 'a';
        char b = 'b';
        System.out.println((int)(b));
        System.out.println((int)(a));
        System.out.println(b-a);

    }   
} 


2
import java.util.*;

public class JavaBasics{
    public static void main(String args[]){
        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        int sum = a+b;

        System.out.println("Sum: " + sum);
    }   
} 


Java 

import java.util.*;


public class JavaBasics{
    public static void main (String args[]){
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter the value for pencil: " );
        float pencil = sc.nextFloat();

        System.out.print("Enter the value for pen: " );
        float pen = sc.nextFloat();
        
        System.out.println("Enter the value for eraser: ");
        float eraser = sc.nextFloat();

        float total = pencil + eraser + pen;
        System.out.println("Total cost is: " + total);

        float newTotal = total + (0.18f * total);
        System.out.println("Bill with 18% tax is: " + newTotal);
    }
}