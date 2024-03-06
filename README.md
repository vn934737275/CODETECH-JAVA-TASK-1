# CODETECH-JAVA-TASK-1
Console-Based Calculator Documentation Using Java
Overview:

The Console-Based Calculator is a Java program designed to perform basic arithmetic operations on two input numbers provided by the user. It operates in a console/command-line interface environment, offering a simple and intuitive way to perform calculations without the need for a graphical user interface.

Features:

-> Supports addition, subtraction, multiplication, and division operations.
-> Utilizes the Scanner class for user input and output.
-> Implements error handling for division by zero and invalid operations.
-> Offers a straightforward and efficient method for performing mathematical calculations.

Installation:

-> Ensure that you have Java installed on your system. If not, download and install Java from the official website: Java Downloads.
->Download the Calculator.java file from the repository.

Compile the Java source code using the Java compiler:

javac Calculator.java

Run the compiled program:

    java Calculator

Usage:
->Upon running the program, the user will be prompted to enter the first number.
->After entering the first number, the user will be prompted to enter the second number.
-> Next, the user will choose the operation to perform (addition, subtraction, multiplication, or division) by entering the corresponding operator (+, -, *, /).
->The program will then display the result of the calculation.
->The user can perform additional calculations by running the program again.

Example:-

sql:

Enter first number: 10
Enter second number: 5
Choose operation (+, -, *, /): *
Result: 50

Error Handling:

    If the user attempts to divide by zero, the program will display an error message ("Error: Division by zero") and terminate gracefully.
    If the user enters an invalid operation, the program will display an error message ("Error: Invalid operation") and terminate gracefully.
    EXPLANATION FOR THE PROGRAM:-
  

    Import Statements:
        import java.util.Scanner;: Imports the Scanner class from the java.util package, which is used to read user input from the console.

    Class Declaration:
        public class Calculator { ... }: Defines a public class named Calculator which contains the main method.

    Main Method:
        public static void main(String[] args) { ... }: The entry point of the program.

    User Input:
        Scanner scanner = new Scanner(System.in);: Creates a new Scanner object named scanner to read user input from the console.
        double num1 = scanner.nextDouble();: Prompts the user to enter the first number and reads it as a double.
        double num2 = scanner.nextDouble();: Prompts the user to enter the second number and reads it as a double.

    Choose Operation:
        char operation = scanner.next().charAt(0);: Prompts the user to choose the operation (+, -, *, /) and reads the first character of the input as a char.

    Perform Operation:
        switch (operation) { ... }: Uses a switch statement to perform the chosen operation based on the user input.
        result = num1 + num2;: Performs addition if the operation is '+'.
        result = num1 - num2;: Performs subtraction if the operation is '-'.
        result = num1 * num2;: Performs multiplication if the operation is '*'.
        result = num1 / num2;: Performs division if the operation is '/', handling division by zero error.

    Output Result:
        System.out.println("Result: " + result);: Displays the result of the calculation.

    Close Scanner:
        scanner.close();: Closes the Scanner object to release system resources.
