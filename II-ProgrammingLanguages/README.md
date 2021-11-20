### Choosing your Programming Language & Getting Started

##### Six Programming Languages and their Uses: Javascript, Python, Java, Swift, C#, C++

| Language   | Why?                                                                                                                                                                                                                                                            |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Javascript | The language of the Web. Powers most of the internet, 100% necesary skill as a programmer. Many flavors, many uses, from SPA, WebApps to Backend Servers.                                                                                                       |
| Python     | One of the best choices for beginner programmers, although it gives a little bit too much freedom. Profesionally used for data sciece, machine learning and deep learning.                                                                                      |
| Java       | Used to be the most widely used worldwide before Javascript took over, widely used for enterprise grade applications, robust, secure and efficient, handles big data like no other. Powers all android devices (although Kotlin seems to be the next big wave). |
| Swift      | The premiere choice for Mac and iOS development, handled and mantained by apple.                                                                                                                                                                                |
| C#         | Microsoft's programming language, powers .NET Core applications, windows desktop applications, Web Assembly based web applications and Unity Games.                                                                                                             |
| C++        | Fastest, most lightweight and efficient language, although pretty steep learning curve, used for game development and large scale data throughputs.                                                                                                             |

##### Functional versus Object Oriented Programming

| Functional Programming                                  | Object Oriented Programming                          |
| ------------------------------------------------------- | ---------------------------------------------------- |
| Emphazises on evaluation of functions, pure and nested. | Based on the concept of objects                      |
| Uses immutable data.                                    | Data is mutable unless said otherwise.               |
| Statements are executed in any order.                   | Statements should be executed in a particular order. |
| Recursion is used for iterative data.                   | Loops are used for iterative data.                   |
| Basic elements include variables and functions.         | Basic elements are objects and methods.              |

##### Constants and Variables

A **constant** is a value that cannot be altered by the program during normal execution, meaning, that value is _constant_. When associated with an identifier, a constant is said to be "named".
A **variable** is a value that can be altered by the program during normal execution.

We can use constants to define variables that may be needed throughout program execution that don't need to change at all. Say we have a program that calculates the area of a circumference.

```
using System;

namespace Circumferences;

class Program
{
    static const double PI = 3.14159;
    public static void Main(string[] args)
    {
        double radiusIntake;
        Console.WriteLine("Provide the radius of a circumference: ");
        radiusIntake = Double.Parse(Console.ReadLine());

        Console.WriteLine($"The area of the circumference is: {CalculateArea(radiusIntake)}");
    }

    private double CalculateArea(double radius)
    {
        return PI * Pow(radius, 2);
    }
}
```

In this example, we use PI as a constant, PI is always _3.1415..._, however, we also have a variable radiusIntake, which changes acording to user input.

##### Identifier Names

Identifier names are descriptive names given to variables and constants in order to make the code more meaningful to us as humans, it is good practice to name your variables according to your code's purpose, having variables that aren't human readable may result in harder to understand and documment code.

Almost all programming languages and coding shops have a standard code formatting style guideline programmers are expected to follow. Among these are three common identifier casing standards:

- camelCase: each word is capitalized except for the first word, no intervening spaces.
- PascalCase: each word is capitalized including the first word, no intervening spaces.
- snake_case: each word is lowercase with underscores separating words.

These are not mandatory, however, they are kinda set in stone so it doesn't hurt just to use them, i.e. C# uses PascalCase for identifiers, whereas Java uses camelCase, and Python uses snake_case.

##### Data Types

A data type is a classification fo data which tells the compiler or interpreter how the programmer intends to use data. Most languages support varios types of data.

| Data Type      | Represents               | Examples                   |
| -------------- | ------------------------ | -------------------------- |
| integer        | whole numbers            | `-5`, `0`, `123`           |
| floating point | fractional numbers       | `-87,45`, `0.0`, `3.14159` |
| string         | a sequence of characters | `"Hello world!"`           |
| boolean        | a logical true or false  | `true`, `false`            |
| nothing        | no data                  | `null`                     |
