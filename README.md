# simple-calculator-with-advance-features_COD4337

TITLE:
CodTech IT Solutions Internship-Task Documentation:Building Simple Calcualtor.

INTRODUCTION:
This documentation provides a detailed explanation of the task assigned during the CodTech IT Solutions internship program.The task involves writing a Java Program to Build Simple calculator .This documentation will cover the implementation details,rationale behind the code structure,and insights into the programming techniques utilized.Additioinally ,it will include information about the intern,Amrapali Sonkamble,and her assigned ID,COD4337.

INTERN INFORMATION:
Name:Amrapali Sonkamble
Intern ID: COD4337

TASK DESCRIPTION:
The task assigned to Amrapali Sonkamble during the CodTech IT Solutions internship program is to Build a Simple Calculator.

IMPLEMENTATION:
The implememtation of the task involves utilizing Java programming language to Build a simple calculator .
'''
import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int choice = 0;

        while (choice != 6) {
            System.out.println("Calculator Menu:");
            System.out.println("1. Addition");
            System.out.println("2. Subtraction");
            System.out.println("3. Multiplication");
            System.out.println("4. Division");
            System.out.println("5. Exponentiation");
            System.out.println("6. Quit");
            System.out.print("Enter your choice: ");
            choice = scanner.nextInt();

            switch (choice) {
                case 1:
                    addition();
                    break;
                case 2:
                    subtraction();
                    break;
                case 3:
                    multiplication();
                    break;
                case 4:
                    division();
                    break;
                case 5:
                    exponentiation();
                    break;
                case 6:
                    System.out.println("Exiting the program...");
                    break;
                default:
                    System.out.println("Invalid choice! Please try again.");
                    break;
            }
        }
        
        scanner.close();
    }

    // Methods for calculator operations

    public static void addition() {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the first number: ");
        double num1 = scanner.nextDouble();
        System.out.print("Enter the second number: ");
        double num2 = scanner.nextDouble();
        double result = num1 + num2;
        System.out.println("Result: " + result);
    }

    public static void subtraction() {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the first number: ");
        double num1 = scanner.nextDouble();
        System.out.print("Enter the second number: ");
        double num2 = scanner.nextDouble();
        double result = num1 - num2;
        System.out.println("Result: " + result);
    }

    public static void multiplication() {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the first number: ");
        double num1 = scanner.nextDouble();
        System.out.print("Enter the second number: ");
        double num2 = scanner.nextDouble();
        double result = num1 * num2;
        System.out.println("Result: " + result);
    }

    public static void division() {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the first number: ");
        double num1 = scanner.nextDouble();
        System.out.print("Enter the second number: ");
        double num2 = scanner.nextDouble();

        if (num2 == 0) {
            System.out.println("Error: Division by zero!");
        } else {
            double result = num1 / num2;
            System.out.println("Result: " + result);
        }
    }

    public static void exponentiation() {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the base: ");
        double base = scanner.nextDouble();
        System.out.print("Enter the exponent: ");
        double exponent = scanner.nextDouble();
        double result = Math.pow(base, exponent);
        System.out.println("Result: " + result);
    }
}

'''

CODE EXPLANATION:
It then takes two numbers as input and performs the selected operation using a switch statement. The result is then displayed on the console.
Please note that this program does not handle input validation, so it assumes that the user will enter valid numbers and make appropriate choices. It also uses the Math.pow() method for exponentiation.
RATIONALE:
1.Importing the necessary package: The program starts by importing the java.util.Scanner package, which allows us to read user input from the console.
    Creating a Scanner object: We create a Scanner object named scanner, which will be used to read user input.
    
2.While loop: We use a while loop to continuously prompt the user for an operation choice until they choose to quit by entering 6.
3.Displaying menu options: Inside the loop, we display a menu of options for the user to choose from, including addition, subtraction, multiplication, division, exponentiation, and the option to quit.
4.Reading user input: We use the nextInt() method of the Scanner object to read the user's choice of operation and store it in the choice variable. We also read the two numbers to perform the operation on using the nextDouble() method.
5. Performing the selected operation: We use a switch statement to perform the selected operation based on the user's choice. Each case of the switch statement calculates the result of the corresponding operation and stores it in the result variable. If the user chooses division, we check if the second number is zero to avoid division by zero error.
6.Displaying the result: We print the result of the operation on the console using System.out.println(). If the user chooses an invalid option, we display an error message.
7.Loop continuation: After displaying the result, we print an empty line to separate the output from the next iteration of the loop.
  
CONCLUSION:
In conclusion the task assigned to Amrapali Sonkamble during CodTech IT solutions internship programming building a simple calculator .The implemented solution successfully accomplishes this task using a 'switch case'.This documentation provides insights ,into the implementation details ,code explanation and rationale behind the chosen approach .Amrapali Sonkamble with the intern ID:COD4337 has effectively completed this task as part of internship programme.
