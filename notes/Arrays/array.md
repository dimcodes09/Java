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

# 4. Linear Search 

import java.util.*;
public class Patterns{

    public static int linearSearch(int numbers[], int key){
        for(int i=0; i<numbers.length; i++){
            if(numbers[i] == key){
                return i;
            }
        }
        return -1;
    }
    public static void main(String[] args){
        int numbers[] ={2,4,6,8,10,12,14,16};
        int key =20;
        int index = linearSearch(numbers, key);
        if(index == -1){
            System.out.println("NOt Found");
        }else{
            System.out.println("Key is at index: " + index);
        }
    } 
}

# 5. Largest Number

import java.util.*;
public class Patterns{

    public static int getLargest(int numbers[]){
        int largest = Integer.MIN_VALUE;
        int smallest = Integer.MAX_VALUE;

        for(int i=0; i<numbers.length; i++){
            if(largest<numbers[i]){
                largest = numbers[i];
            }
            if(smallest > numbers[i]){
                smallest = numbers[i];
            }
        }
        System.out.println("The smallest number is: " + smallest);
        return largest;
    }
    public static void main(String[] args){
        int numbers[] ={1,2,6,3,5};
        System.out.println("Largest value is: " + getLargest(numbers));
    }
} 