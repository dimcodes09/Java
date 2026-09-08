


public class JavaBasics{
    public static void main (String args[]){
        int age = 16;
        if(age>= 18){
            System.out.println("Adult: drive, vote");
        }
            if(age > 13 && age < 18){
                System.out.println("Teenager");
            }
        else{
            System.out.println("not adult");
        }
        

    }
}


# To Check Odd or EVen

import java.util.*;

public class JavaBasics{
    public static void main (String args[]){
        Scanner sc = new Scanner(System.in);
        int number = sc.nextInt();
        if(number % 2 == 0){
            System.out.println("EVEN");
        }else{
            System.out.println("ODD");
        }
    }
}

# else if Ststements


public class JavaBasics{
    public static void main (String args[]){
        int age = 19;
        if(age>=18){
            System.out.println("adult");
        }else if (age>=13 && age<18){
            System.out.println("Teenager");
        }else{
            System.out.println("Adult");
        }
    }
}

# Income Tax Calculator

import java.util.*;

public class JavaBasics{
    public static void main (String args[]){
        Scanner sc = new Scanner(System.in);
        int income = sc.nextInt();
        int tax;

        if(income< 500000){
            tax = 0;
        }
        else if(income >= 500000 && income <1000000){
            tax = (int) (income * 0.2);
        }else{
            tax = (int) (income * 0.3);
        }
        System.out.println("your tax is : " + tax);
    }
}

# LArgest among three numbers

public class JavaBasics{
    public static void main (String args[]){
        int A=1;
        int B =3;
        int C=6;
        if((A >= B) && (A >= C)){
            System.out.println("LArgest is A");
        }else if(B >= C){
            System.out.println("LArgest is B");
        }else{
            System.out.println("LArgest is C");
        }
    }
}