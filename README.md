# java.util.Scanner
java.util.Scanner
import java.util.Scanner;

public class Factorial {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Введите число: ");
        int number = scanner.nextInt();
        
        int factorial = calculateFactorial(number);
        
        System.out.println("Факториал числа " + number + " равен " + factorial);
    }
    
    public static int calculateFactorial(int number) {
        if (number == 0 || number == 1) {
            return 1;
        } else {
            return number * calculateFactorial(number - 1);
        }
    }
}
