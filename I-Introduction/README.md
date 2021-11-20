### Introduction to Programming

- Systems Development Life Cycle
- Program Design
- Pseudocode
- Integrated Development Environment
- Version Control
- Hello World!

---

### Systems Development Life Cycle

> Planning -> Analysis -> Design -> Implementation -> Maintenance

---

### Program Design

1. Understanding the Problem - Figuring out the Program
2. Usign design tools to create a Model
3. Develop test data

A program should be:

- Reliable (how often results in the program are the ones expected)
- Robust (how well the program anticipates and handles human error)
- Usable (how ergonomic/easy to use a program is)
- Portable (range of computer hardware the program can run in)
- Maintanable (how easy the program is to mantain)
- Efficient (how fast/performing a program is)
- Readable (easy to read and understand source code)

> Keywords: abstraction, inputs, outputs

---

### Pseudocode

Pseudocode is an informal high-level description of the operating principle of a computer program or algorithm.

After developing the program design,we use **pseudocode** to write code in a language where you must follow the rules of said language (syntax) in order to code the logic or algorithm presented in the pseudocode.

```
Input
    display a message asking the user to enter the first age
    get the first age from the keyboard
    display a message asking the user to enter the second age
    get the second age from the keyboard
Processing
    calculate the answer by adding the two ages together and dividing by two
Output
    display the answer on the screen
    pause so the user can see the answer
```

Translates to (in C# 10.X)

```
namespace sample;

class Program
{
    public static void Main(string[] args)
    {
        //Input
        int firstAge, secondAge;
        Console.WriteLine("Provide the first age: ");
        firstAge = int.Parse(Console.ReadLine());

        Console.WriteLine("Provide the second age: ");
        secondAge = int.Parse(Console.ReadLine());

        //Processing
        int avgAge = (firstAge + secondAge) / 2;

        //Output
        Console.WriteLine($"The average age is: {avgAge}")
    }
}
```

### Integrated Development Environment

An **integrated development environment (IDE)** is a software application that provides facilities to computer programmers for software development. An IDE consists usually of a source code editor, build automation tools, a debugger and sometimes: intelligent code completion. Some IDEs also have a compiler or interpreter, or both. Amongside other tools such as external plugins, source control versioning, file explorer and hierarchy diagrams.

### Version Control

Version, revision or source control is the management of changes to documents, computer programs, websites or any collection of information that belongs to a given project repository. Each revision is associated with a timestamp and an author whom made the change. Revisions can be compared, restored or merged as needed.

**Git** is the leading version control system across the globe, it makes tracking changes and coordinated work among files easy to read and understand, Git was created in 2005 by Linus Tovalds and it consists of a series of easy to understand keywords that help populate and work with a repository.

### Hello World!

Hello World is the first program every programmer has to write, it is a rite of passage and it serves the purpose of giving explaination on how different languages have different syntaxes, but all have the same objective, to write "hello world". Let's see

##### C++

```
#include

int main()
{
    std::cout << "Hello, world!";
    return 0;
}
```

##### C#

```
namespace Program;
class Program
{
    public static void main(string[] args)
    {
        Console.WriteLine("Hello World!");
    }
}
```

##### Javascript

```
console.log('Hello World!');
```

##### Pascal

```
program HelloWorld;
begin
    WriteLn('Hello world!');
end.
```

##### Python

```
print "Hello world!"
```

##### Java

```
public class HelloWorld {
    public static void main(string[] args){
        System.out.printLn("Hello World!");
    }
}
```

##### SQL

```
SELECT "Hello World" FROM tempdb;
```

##### Bash

```
echo "Hello World!"
```
