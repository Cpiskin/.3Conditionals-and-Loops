# 1.3Conditionals-and-Loops

import java.util.Random;

public class RollLoadedDie {

    public static void main(String[] args) {
        // Define the probabilities
        double p1 = 1.0/8;
        double p2 = 2.0/8;
        double p3 = 3.0/8;
        double p4 = 4.0/8;
        double p5 = 5.0/8;
        double p6 = 1.0;

        // Create an instance of Random
        Random random = new Random();

        // Generate a random number between 0 (inclusive) and 1 (exclusive)
        double rand = random.nextDouble();

        // Find the outcome based on the probabilities
        if (rand < p1) {
            System.out.println("You rolled: 1");
        } else if (rand < p2) {
            System.out.println("You rolled: 2");
        } else if (rand < p3) {
            System.out.println("You rolled: 3");
        } else if (rand < p4) {
            System.out.println("You rolled: 4");
        } else if (rand < p5) {
            System.out.println("You rolled: 5");
        } else {
            System.out.println("You rolled: 6");
        }
    }
}
