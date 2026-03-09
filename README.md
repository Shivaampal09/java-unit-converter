import java.util.Scanner;

public class UnitConverterTool {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("===== UNIT CONVERTER TOOL =====");
        System.out.println("1. Meter to Kilometer");
        System.out.println("2. Celsius to Fahrenheit");
        System.out.println("3. Kilogram to Gram");
        System.out.print("Choose option: ");

        int choice = sc.nextInt();

        switch (choice) {

            case 1:
                System.out.print("Enter meters: ");
                double meter = sc.nextDouble();
                System.out.println("Kilometers: " + (meter / 1000));
                break;

            case 2:
                System.out.print("Enter Celsius: ");
                double c = sc.nextDouble();
                System.out.println("Fahrenheit: " + ((c * 9/5) + 32));
                break;

            case 3:
                System.out.print("Enter Kilogram: ");
                double kg = sc.nextDouble();
                System.out.println("Gram: " + (kg * 1000));
                break;

            default:
                System.out.println("Invalid option");
        }

        sc.close();
    }
}
