import java.util.Scanner;

public class TextAdventureGame {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Welcome to the Text Adventure Game!");

        // TODO: Implement your game logic and story here

        scanner.close();
    }

    // TODO: Define methods for different decision points and outcomes
    // Example:
    private static void makeDecision1() {
        System.out.println("You come across a fork in the road. Do you go left or right?");
        String decision = getUserInput();
        
        // TODO: Implement logic for the outcome based on the user's decision
        // Example:
        if (decision.equalsIgnoreCase("left")) {
            System.out.println("You find a hidden treasure!");
        } else if (decision.equalsIgnoreCase("right")) {
            System.out.println("You encounter a friendly dragon.");
        } else {
            System.out.println("Invalid input. Please try again.");
            makeDecision1(); // Recursively call the method for valid input
        }
    }

    // TODO: Define more methods for different decision points

    private static String getUserInput() {
        System.out.print("Enter your decision: ");
        Scanner scanner = new Scanner(System.in);
        return scanner.nextLine();
    }
}
