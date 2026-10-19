import java.util.*;

public class JavaBasics {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first integer: ");
        float one = sc.nextFloat();

        System.out.print("Enter second integer: ");
        float second = sc.nextFloat();

        float sum = one + second;
        System.out.println("Sum = " + sum);

        float Difference = second - one;
        System.out.println("Difference = " + Difference);

        float Product = one * second;
        System.out.println("Product = " + Product);

        float Quotient = one / second;
        System.out.println("Quotient = " + Quotient);

        float Remainder = one % second;
        System.out.println("Remainder = " + Remainder);



    }
}