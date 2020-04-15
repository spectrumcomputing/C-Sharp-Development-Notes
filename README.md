# C-Sharp-Development-Notes

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
