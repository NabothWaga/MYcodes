# MYcodes
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Enter the number of elements in the array:");
        int n = scanner.nextInt();

        int[] array = new int[n];

        System.out.println("Enter the elements of the array:");
        for (int i = 0; i < n; i++) {
            array[i] = scanner.nextInt();
        }

        System.out.println("Enter the index of the element you want to access:");
        int index = scanner.nextInt();

        try {
            System.out.println("The element at index " + index + " is: " + array[index]);
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Error: Index " + index + " is out of bounds.");
        }
    }
}
