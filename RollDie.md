//Write a program RollDie.java that generates the result of rolling a fair six-sided die (an integer between 1 and 6).


import java.util.Random;

public class RollDie {

    public static void main(String[] args) {
        // Create an instance of Random
        Random random = new Random();

        // Generate a random number between 1 and 6 (inclusive)
        int result = random.nextInt(6) + 1;

        System.out.println("You rolled: " + result);
    }
}
