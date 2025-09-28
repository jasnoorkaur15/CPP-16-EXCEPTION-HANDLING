# Experiemnt-16: Exception Handling

## AIM

To understand and implement exception handling in C++ using the try, throw, and catch mechanism through the following programs:

Division of two numbers (with division by zero check)

Age validation (checking if the user is underage)

## OBJECTIVES

To learn how C++ handles runtime errors gracefully.

To understand the use of try, throw, and catch blocks.

To practice throwing exceptions of different data types.

To explore exception handling as an alternative to traditional error handling using conditions.

To ensure program safety and reliability during abnormal situations.

## THEORY
### What is Exception Handling?

Exception handling is a mechanism to detect and handle runtime errors in a structured way.

Instead of terminating the program abruptly when an error occurs, exceptions allow the program to “catch” the error and respond to it.

### Need for Exception Handling

Runtime errors such as division by zero, invalid input, file not found, or out of range access can cause program crashes.

Traditional error handling using conditions (like if statements) may not be sufficient in complex programs.

Exception handling provides a structured, safer, and cleaner way to deal with such issues.

Components of Exception Handling

#### try block:

Contains the code where an exception might occur.

If an exception happens, control is transferred to the matching catch block.

#### throw statement:

Used to signal that an exception has occurred.

It can throw values of any data type (e.g., int, float, string, object).

#### catch block:

Handles the exception thrown by throw.

Different catch blocks can handle different types of exceptions.

Advantages of Exception Handling

Improves program reliability and security.

Separates error-handling code from normal program logic.

Handles unexpected events without crashing the program.

Allows multiple types of errors to be handled in one program.

## Exception Handling vs Normal Error Handling
| Feature        | Normal Error Handling (if-else)     | Exception Handling (try-throw-catch)       |
| -------------- | ----------------------------------- | ------------------------------------------ |
| Style          | Mixes error checks with logic       | Separates logic and error-handling clearly |
| Flexibility    | Limited, must check conditions      | Can handle multiple error types gracefully |
| Runtime Errors | May cause crash if unhandled        | Prevents crash by handling errors safely   |
| Readability    | Code may become lengthy and complex | Cleaner and structured                     |

## COMPARISON TABLE
| Program          | Exception Condition    | Exception Type | Example Input   | Example Output       | Concept Focus            |
| ---------------- | ---------------------- | -------------- | --------------- | -------------------- | ------------------------ |
| Division Program | If denominator is zero | float          | n1 = 10, n2 = 0 | ERROR: Division by 0 | Mathematical error check |
| Age Validation   | If age < 18            | int            | age = 15        | ERROR: Underage (15) | Input validation         |

## Algorithms
### Algorithm for Division Program (Division by Zero Check)

Start.

Input two numbers: numerator and denominator.

Begin a try block.

If denominator = 0 → throw an exception.

Else → perform division and display the result.

In the catch block, handle the exception by displaying "ERROR: Division by 0".

Stop.

### Algorithm for Age Validation Program

Start.

Input age.

Begin a try block.

If age < 18 → throw an exception (underage).

Else → display valid age and approval message.

In the catch block, handle the exception by displaying "ERROR: Underage".

Stop.

## PROGRAM DESCRIPTIONS
### Division Program (Division by Zero Check)

Aim: To perform division of two numbers with exception handling for division by zero.

Logic:

Input two numbers.

If the second number is zero, throw an exception.

Otherwise, perform division and display the result.

Concept Focus: Runtime error handling for mathematical operations.

### Age Validation Program

Aim: To validate age using exception handling.

Logic:

Input an age value.

If the age is less than 18, throw an exception (underage).

Otherwise, display the age and approval message.

Concept Focus: Input validation with exceptions.

## CONCEPTS USED

Exception Handling Mechanism: Central to both programs.

try, throw, catch: Key keywords in C++ exception handling.

Runtime Error Checking: Prevents division by zero and underage approval.

Data Type Specific Exceptions: Float exception in division program, integer exception in age program.

Program Safety: Prevents unexpected program crashes.

## CONCLUSION

Exception handling is a powerful tool in C++ for writing safe and reliable programs.

The division program demonstrates how to avoid mathematical errors like division by zero.

The age validation program highlights how exceptions can be used for logical input checks.

By separating error-handling code from normal execution, exception handling improves program clarity and prevents crashes.

It is particularly useful in large applications where multiple types of errors may occur


