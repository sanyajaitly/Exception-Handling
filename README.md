# Exception-Handling

AIM

Exception-Handling

THEORY

C++ Exceptions

When executing C++ code, different errors can occur: coding errors made by the programmer, errors due to wrong input, or other unforeseeable things.

When an error occurs, C++ will normally stop and generate an error message. The technical term for this is: C++ will throw an exception (throw an error).

C++ try and catch

Exception handling in C++ consist of three keywords: try, throw and catch:

The try statement allows you to define a block of code to be tested for errors while it is being executed.

The throw keyword throws an exception when a problem is detected, which lets us create a custom error.

The catch statement allows you to define a block of code to be executed, if an error occurs in the try block.

The try and catch keywords come in pairs:

Example

try {

// Block of code to try

throw exception; // Throw an exception when a problem arise

}

catch ()

{

// Block of code to handle errors

}

C++ Standard Exceptions

C++ provides a list of standard exceptions defined in which we can use in our programs. These are arranged in a parent-child class hierarchy shown below −

C++ Exceptions Hierarchy




ALGORITHM

Part-A
The code you provided is a C++ program that performs division of two numbers, a and b, and uses exception handling to catch and handle the case where b is equal to 0.

Here's a breakdown of how the code works:

1.It declares three integer variables: a, b, and c.

2.It prompts the user to enter two numbers using cout.

3.It reads the two numbers into a and b using cin.

4.It checks if b is not equal to 0 using an if statement.

5.If b is not equal to 0, it performs the division of a by b and stores the result in c. Then, it prints the result using cout.

6.If b is equal to 0, it throws an exception with the value of b.

7.It catches the exception using a catch block that specifies the exception type as int, meaning it will catch exceptions of type int.

8.Inside the catch block, it prints an error message indicating that division by the value of b (which is 0) is not allowed.

9.In your provided example, when the user enters "2" for a and "0" for b, the program correctly detects that b is equal to 0 and throws an exception. The exception is caught in the catch block, and the program prints the error message "Divide by 0 error."

10.So, the output you provided is expected and demonstrates the proper functioning of the exception handling mechanism in C++.

Part-B
The code you provided is a C++ program that takes a user's age as input and uses exception handling to determine whether the person is eligible based on their age. Here's the algorithm of how the code works:

1.Declare an integer variable a to store the age.

2.Display a message using cout to prompt the user to enter their age.

3.Read the user's input into the variable a using cin.

4.Use a try block to begin exception handling.

5.Inside the try block, check if the value of a is greater than or equal to 18 using an if statement.

6.If a is greater than or equal to 18, it means the person is eligible, so print a message using cout indicating eligibility along with their age.

7.If a is less than 18, it means the person is not eligible, so throw an exception with the value of a.

8.Use a catch block to catch the exception. In this case, the exception type specified is int, meaning it will catch exceptions of type int.

9.Inside the catch block, print an error message indicating that the person is not eligible, along with the word "error."

10.Finally, return 0 to indicate successful program execution.

The code's purpose is to check if the age entered by the user is 18 or older. If it is, the program informs the user that they are eligible. If the age is less than 18, an exception is thrown and caught to display an error message indicating that the person is not eligible.
