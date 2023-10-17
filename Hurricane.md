

import java.util.Scanner;
public class Hurricane {

    public static void main(String[] args) {
    
        Scanner s = new Scanner(System.in);

        System.out.println("Enter the wind speed in miles");
        int windspeed = s.nextInt();

        if (windSpeed >= 74 && windSpeed <= 95) {
            System.out.println("Category 1 Hurricane");
        } else if (windSpeed >= 96 && windSpeed <= 110) {
            System.out.println("Category 2 Hurricane");
        } else if (windSpeed >= 111 && windSpeed <= 130) {
            System.out.println("Category 3 Hurricane");
        } else if (windSpeed >= 131 && windSpeed <= 155) {
            System.out.println("Category 4 Hurricane");
        } else if (windSpeed >= 156) {
            System.out.println("Category 5 Hurricane");
        } else {
            System.out.println("Not a hurricane.");
        }
    }
}
