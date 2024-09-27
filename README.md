``` c#
using System;
using System.Collections.Generic;
using System.Globalization;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._2._9RandomNumberGeneration
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Random r = new Random(); // always at the start of the program
            Console.WriteLine(r.Next(1, 100)); // Numbers from 1 to 99 included in possible outcomes
            int a, b, c;
            a = r.Next(1,50);
            b = r.Next(50,150);
            c = r.Next(991, 3201);
            Console.WriteLine($"{a} {b} {c}");
            Console.WriteLine(a + b + c);
            for(int i = 0; i < 10; i++)
            {
                Console.WriteLine(r.Next(1, 10));
            }
            
        }
        int FunctionUsingRandom(Random n,int max)
        {
            return (n.Next(0, max));
        }
    }
}
```
