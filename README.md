# C-Sharp-Development-Notes

### Data Types

```cs
static void Main(string[] args)
{
        string name = "Mike";    // String's are objects not primitives
        char testGrade = 'A';    // single 16-bit Unicode character.

        // short, int, long can be pre-pended with 'u' for 'unsigned'
        byte age0 = 0;           // 8-bit unsigned integer
        short age1 = 10;         // 16-bit signed integer.
        int age2 = 20;           // 32-bit signed integer
        long age3 = 30L;         // 64-bit signed integer

        float gpa0 = 2.5F;       // 32-bit floating point
        double gpa1 = 3.5;       // 64-bit double-precision floating point
        decimal gpa2 = 4.5M;     // 128-bit precise decimal

        bool isTall;             // 1 bit -> true/false
        isTall = true;

        name = "John";

        Console.WriteLine("Your name is " + name);
        Console.WriteLine($"Your name is {name}");
}
```
https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/floating-point-numeric-types

### Strings

```cs
static void Main(string[] args)
{
        string greeting = "Hello";
        //      indexes:   01234

        Console.WriteLine(greeting.Length);          // 5
        Console.WriteLine(greeting[0]);              // H
        Console.WriteLine(greeting.IndexOf("llo"));  // 2
        Console.WriteLine(greeting.IndexOf("z"));    // -1
        Console.WriteLine(greeting.Substring(2));    // llo
        Console.WriteLine(greeting.Substring(1, 3)); // ell
}
```

https://docs.microsoft.com/en-us/dotnet/api/system.string.indexof

https://docs.microsoft.com/en-us/dotnet/api/system.string.substring

### Arrays

```cs
static void Main(string[] args)
{
        int [] luckyNumbers = new int[10];
        luckyNumbers[0] = 90;
            
        Console.WriteLine(luckyNumbers[0]);
        Console.WriteLine(luckyNumbers[1]);
        Console.WriteLine(luckyNumbers.Length);
}
 ```
 
 ```cs
static void Main(string[] args)
{
    int[] luckyNumbers = { 4, 8, 15, 16, 23, 42 };
    luckyNumbers[0] = 90;

    Console.WriteLine(luckyNumbers[0]);
    Console.WriteLine(luckyNumbers[1]);
    Console.WriteLine(luckyNumbers.Length);
}
 ```
 https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/arrays/

### While & Do-While Loops

```cs
        static void Main(string[] args)
        {

            // The while loops test the condition before executing commands

            int index = 1;
            while (index <= 5)
            {
                Console.WriteLine(index);
                index++;
            }

            Console.WriteLine();

            // The do-while loop executes the code at least once
            do
            {
            Console.WriteLine(index);
            index++;
            }
            while(index <= 5);
        }
```
https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/while

https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/do

### If-Else Branching

```cs
        static void Main(string[] args)
        {
            bool isStudent = false;
            bool isSmart = false;

            if (isStudent && isSmart)
            {
                Console.WriteLine("You are a student");
            }
            else if (isStudent && !isSmart)
            {
                Console.WriteLine("You are not a smart student");
            }
            else
            {
                Console.WriteLine("You are not a student and not smart");
            }

            // >, <, >=, <=, !=, ==
            if (1 < 3)
            {
                Console.WriteLine("number omparison was true");
            }
        }
```
https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/if-else

### Methods

```cs
        static void Main(string[] args)
        {
            int sum = AddNumbers(4, 60);
            Console.WriteLine(sum);
        }

        public static int AddNumbers(int num1, int num2)
        {
            return num1 + num2;
        }
```
https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/methods


 
