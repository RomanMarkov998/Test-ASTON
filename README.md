# Test-ASTON
import java.util.Scanner;
public class Calculator {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Ввод двух целых чисел
        System.out.print("Введите число a: ");
        int a = scanner.nextInt();

        System.out.print("Введите число b: ");
        int b = scanner.nextInt();

        // Сравнение и вывод результата
        compareNumbers(a, b);

        // Операции сложения, вычитания, деления и умножения
        performOperations(a, b);
    }

    private static void compareNumbers(int a, int b) {
        // Сравнение чисел
        if (a > b) {
            System.out.println("a > b");
        } else if (a < b) {
            System.out.println("a < b");
        } else {
            System.out.println("a = b");
        }
    }

    private static void performOperations(int a, int b) {
        // Операции сложения, вычитания, деления и умножения
        System.out.println("Сложение (a + b): " + (a + b));
        System.out.println("Вычитание (a - b): " + (a - b));

        if (b != 0) {
            System.out.println("Деление (a / b): " + ((double) a / b));
        } else {
            System.out.println("Деление на ноль невозможно");
        }

        System.out.println("Умножение (a * b): " + (a * b));
    }
}
