# solved-coding-questions
solving top 100 codes in 100 days 

Write a Java program to find the second largest and second smallest elements in an array without sorting.
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

1️⃣ Find the Maximum and Minimum in an Array
Question:
Write a Java program to find the maximum and minimum values in an array.

Code:
java
Copy
Edit
class Main {
    public static void main(String args[]) {
        int a[] = {1, 2, 34, 4, 5, 6, 7};  
        
        int max = a[0], min = a[0];

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
Output:
Max: 34  
Min: 1  
2️⃣ Find the Second Largest Element in an Array
Question:
Write a Java program to find the second largest element in an array without sorting.

Code:

class Main {
    public static void main(String args[]) {
        int a[] = {1, 2, 34, 4, 5, 6, 7};  
        
        int max = Integer.MIN_VALUE, secondMax = Integer.MIN_VALUE;

        for (int i = 0; i < a.length; i++) {
            if (a[i] > max) {
                secondMax = max;
                max = a[i];
            } else if (a[i] > secondMax && a[i] != max) {
                secondMax = a[i];
            }
        }

        System.out.println("Second Largest: " + secondMax);
    }
}
Output:

Second Largest: 7  
3️⃣ Find the Second Smallest Element in an Array
Question:
Write a Java program to find the second smallest element in an array without sorting.

Code:

class Main {
    public static void main(String args[]) {
        int a[] = {1, 2, 34, 4, 5, 6, 7};  
        
        int min = Integer.MAX_VALUE, secondMin = Integer.MAX_VALUE;

        for (int i = 0; i < a.length; i++) {
            if (a[i] < min) {
                secondMin = min;
                min = a[i];
            } else if (a[i] < secondMin && a[i] != min) {
                secondMin = a[i];
            }
        }

        System.out.println("Second Smallest: " + secondMin);
    }
}
Output:

Second Smallest: 2  
4️⃣ Find Maximum, Minimum, Second Largest, and Second Smallest
Question:
Write a Java program to find the maximum, minimum, second largest, and second smallest elements in an array.

Code:

class Main {
    public static void main(String args[]) {
        int a[] = {1, 2, 34, 4, 5, 6, 7};  
        
        int max = Integer.MIN_VALUE, secondMax = Integer.MIN_VALUE;
        int min = Integer.MAX_VALUE, secondMin = Integer.MAX_VALUE;

        for (int i = 0; i < a.length; i++) {
            if (a[i] > max) {
                secondMax = max;
                max = a[i];
            } else if (a[i] > secondMax && a[i] != max) {
                secondMax = a[i];
            }

            if (a[i] < min) {
                secondMin = min;
                min = a[i];
            } else if (a[i] < secondMin && a[i] != min) {
                secondMin = a[i];
            }
        }

        System.out.println("Max: " + max);
        System.out.println("Min: " + min);
        System.out.println("Second Largest: " + secondMax);
        System.out.println("Second Smallest: " + secondMin);
    }
}
Output:

Max: 34  
Min: 1  
Second Largest: 7  
Second Smallest: 2  

output :

Max: 34  
Second Max: 7  
Min: 1  
Second Min: 2  
