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

### Strings

```cs
  static void Main(string[] args)
        {
            string greeting = "Hello";
            //      indexes:   01234

            Console.WriteLine(greeting.Length);
            Console.WriteLine(greeting[0]);
            Console.WriteLine(greeting.IndexOf("llo"));
            Console.WriteLine(greeting.IndexOf("z"));
            Console.WriteLine(greeting.Substring(2));
            Console.WriteLine(greeting.Substring(1, 3));
        }
```

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
