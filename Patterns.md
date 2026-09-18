# Reverse Pattern

public static void main (String args[]){
    int n =4;
    for(int line = 1 ; line <= 5; line++){
        for(int star=1; star<=n-line+1; star++){
            System.out.print("*");
        }
        System.out.println();
    }
}


# Hollow rectangle

public class Patterns{
    public static void hollow_rectangle(int totRows, int totCols){
        for (int i = 1; i<=totRows; i++){
            //iinner - coloumns
            for(int j=1; j<=totCols; j++){
                if(i==1 || i == totRows || j==1 || j == totCols){
                    System.out.print('*');
                }else{
                    System.out.print(" ");
                }
            }
            System.out.println();
        }
    }
    public static void main(String args[]){
        hollow_rectangle(10, 7);
    }
} 

