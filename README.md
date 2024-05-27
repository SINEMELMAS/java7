# java7
package lab2;
import java.util.Scanner;
public class Addition {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Please enter number of values to sum: ");
        int numberOfValues = scanner.nextInt();

        int sum = 0;
        int count = 0;

        do {
            System.out.print("Enter a number: ");
            int num = scanner.nextInt();
            sum += num;
            count++;
        } while (count < numberOfValues);

        System.out.println("Sum of the numbers: " + sum);

        scanner.close();
    }
}
