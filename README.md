# solved-coding-questions
solving top 100 codes in 100 days 
import java.util.Scanner;

class Main {
    public static void main(String args[]) {
        int a[] = {1, 2, 34, 4, 5, 6, 7};  
        
        int max = a[0];  
        int min = a[0];  

        for (int i = 1; i < a.length; i++) {
            if (a[i] > max) {
                max = a[i];  
            }
            if (a[i] < min) {
                min = a[i];  
            }
        }

        System.out.println("Max: " + max);
        System.out.println("Min: " + min);
    }
}
