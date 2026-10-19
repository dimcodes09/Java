# to calc % & print marks

import java.util.*;
public class Patterns{

    public static void main(String[] args){
        int marks[] = new int[50];

        Scanner sc = new Scanner(System.in);

        // System.out.println("length of array = " + marks.length);
        marks[0]= sc.nextInt();
        marks[1]= sc.nextInt();
        marks[2]= sc.nextInt();

        System.out.println("phy: " + marks[0]);
        System.out.println("chem: " + marks[1]);
        System.out.println("math: " + marks[2]);

        // marks[2] = marks[2] + 1;
        // System.out.println("math: " + marks[2]);

        int percentage = (marks[0] + marks[1] + marks[2]) /3;
        System.out.println("percentage =" + percentage + "%");

    } 
}


# 2. to calc length of array

import java.util.*;
public class Patterns{

    public static void main(String[] args){
        int marks[] = new int[50];

        Scanner sc = new Scanner(System.in);

        // System.out.println("length of array = " + marks.length);

    }
}

# 3. Passign array as an argument

import java.util.*;
public class Patterns{

    public static void update(int marks[], int nonChangable){
        nonChangable = 10;
        for(int i=0; i<marks.length; i++){
            marks[i] = marks[i] + 1;
        }
    }

    public static void main(String[] args){
        int marks[]= {97,98,99};
        int nonChangable = 5;
        update(marks , nonChangable);
        System.out.println(nonChangable);

        //print our marks
        for(int i=0; i<marks.length; i++){
            System.out.print(marks[i] + " ");
        }
        System.out.println();
    } 
}

# 4. 