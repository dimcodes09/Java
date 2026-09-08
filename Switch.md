# your fav


public class JavaBasics{
    public static void main (String args[]){
        int ch = 'a';
        switch(ch){
            case 'd': System.out.println("Samosa");
            break;
            case 'a': System.out.println("Banana");
            break;
            case 'b': System.out.println("Mango Shake");
            break;
            default: System.out.println("Wake up to Reality");
            break;
        }
    }
}



# Calculator

public class JavaBasics{
    public static void main (String args[]){
        int ch = 'a';
        switch(ch){
            case 'd': System.out.println("Samosa");
            break;
            case 'a': System.out.println("Banana");
            break;
            case 'b': System.out.println("Mango Shake");
            break;
            default: System.out.println("Wake up to Reality");
            break;
        }
    }
}

# Week Days

import java.util.*;

public class JavaBasics{
    public static void main (String args[]){
        Scanner sc = new Scanner(System.in) ;
        System.out.println("Enter week number from 1-7");
        int week = sc.nextInt();

        switch(week){
            case 1:
                System.out.println("Monday");
                break;
                case 2:
                System.out.println("Tue");
                break;
                case 3:
                System.out.println("Wed");
                break;
                case 4:
                System.out.println("THu");
                break;
                case 5:
                System.out.println("Fri");
                break;
                case 6:
                System.out.println("Sat");
                break;
                case 7:
                System.out.println("Sun");
                break;
                default: 
                System.out.println("Please enter a valid week day from 1-7");
        }
        }
    }



