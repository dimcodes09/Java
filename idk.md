import java.util.Scanner;

public class JavaBasics{
    public static void main (String args[]){
       Scanner sc = new Scanner(System.in);

       int number;
       int choice;
       int evenSum = 0;
       int oddSum = 0;

       do { 
           System.out.print("Enter the Number: ");
           number = sc.nextInt();

           if(number % 2 == 0){
            evenSum += number;
           }else{
            oddSum += number;
           }
           System.out.println("Do you want to continue Press 0 to stop and 1 to continue");
           choice = sc.nextInt();
       } while (choice == 1);
       System.out.println("Sum of even Numbers: " + evenSum);
       System.out.println("Summ of odd numbers: " + oddSum);
    }
    }