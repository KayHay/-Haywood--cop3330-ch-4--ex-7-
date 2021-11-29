# -Haywood--cop3330-ch-4--ex-7-
Chapter 4, Exercise 7

/*
 *  UCF COP3330 Fall 2021 Assignment 5 Solution
 *  Copyright 2021 Kaylah Haywood
 */
 
import java.util.Scanner;

class Main {
  public static void main(String[] args) {

    char operator;
    Double number1, number2, result;

    // Creating Scanner class object
    Scanner input = new Scanner(System.in);

    // User operator input
    System.out.println("Select an operator: +, -, *, or /");
    operator = input.next().charAt(0);

    // User numbers input
    System.out.println("Enter the first number");
    number1 = input.nextDouble();

    System.out.println("Enter the second number");
    number2 = input.nextDouble();

    switch (operator) {

      // Addition performance
      case '+':
        result = number1 + number2;
        System.out.println(number1 + " + " + number2 + " = " + result);
        break;

      // Subtraction performance
      case '-':
        result = number1 - number2;
        System.out.println(number1 + " - " + number2 + " = " + result);
        break;
        
      // Multiplication performance
      case '*':
        result = number1 * number2;
        System.out.println(number1 + " * " + number2 + " = " + result);
        break;

      // Division performance
      case '/':
        result = number1 / number2;
        System.out.println(number1 + " / " + number2 + " = " + result);
        break;

      default:
        System.out.println("The operator is invalid!");
        break;
    }

    input.close();
  }
}
