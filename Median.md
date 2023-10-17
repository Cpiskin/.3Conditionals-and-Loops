// Write a program that takes five integer command-line arguments and prints the median (the third largest one).

import java.util.Scanner;
public class Median {

    public static void main(String[] args) {
        // Assuming exactly five integers are provided as command-line arguments

        Scanner s = new Scanner(System.in);

        System.out.println("Enter number 1");
        int num1 = s.nextInt();
        System.out.println("Enter number 2");
        int num2 = s.nextInt();
        System.out.println("Enter number 3");
        int num3 = s.nextInt();
        System.out.println("Enter number 4");
        int num4 = s.nextInt();
        System.out.println("Enter number 5");
        int num5 = s.nextInt();

        int median;

        // Find the median
        if (num1 >= num2 && num1 <= num3 || num1 <= num2 && num1 >= num3) {
            median = num1;
        } else if (num2 >= num1 && num2 <= num3 || num2 <= num1 && num2 >= num3) {
            median = num2;
        } else {
            median = num3;
        }

        if (num4 >= median) {
            if (num4 >= num5) {
                median = num4;
            } else if (num5 >= median) {
                median = num5;
            }
        } else if (num5 >= median) {
            median = num5;
        }

        System.out.println("The median is: " + median);
    }
}
