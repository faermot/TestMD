<img src="https://github.com/user-attachments/assets/f57852aa-b866-4a98-b1f2-5788c74bcd49" width="135" />

<img src="https://github.com/user-attachments/assets/d423572f-49d6-4d3d-af2a-02381d6e2863" width="145" />

<img src="https://github.com/user-attachments/assets/935e84bd-b952-4747-a70d-223b74a3a17e" width="145" />

Main
```csharp
using ConsoleApp19.Utils;
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading;
using System.Threading.Tasks;

namespace ConsoleApp19
{
    internal class Program
    {
        static void Main(string[] args)
        {
            while (true)
            {
                Console.Clear();
                Console.Write("Выберите задание (1-30): ");
                switch (Console.ReadLine())
                {
                    case "1":
                        {
                            Console.Clear();
                            Console.WriteLine("Задание №1");

                            Task1[] points = { new Task1(3.5, 7.2),  new Task1(-0.5, 1.2), new Task1(0.72, -3.12)};

                            if (points[0].IsInArea()) Console.WriteLine($"Точка A ({points[0].X}, {points[0].Y}) лежит в области");
                            else Console.WriteLine($"Точка A ({points[0].X}, {points[0].Y}) НЕ лежит в области");


                            if (points[1].IsInArea()) Console.WriteLine($"Точка A ({points[0].X}, {points[0].Y}) лежит в области");
                            else Console.WriteLine($"Точка A ({points[1].X}, {points[1].Y}) НЕ лежит в области");

                            if (points[2].IsInArea()) Console.WriteLine($"Точка A ({points[0].X}, {points[0].X}) лежит в области");
                            else Console.WriteLine($"Точка A ({points[1].X}, {points[1].Y}) НЕ лежит в области");


                            Console.ReadKey();
                        }
                        break;

                    case "2":
                        {
                            Console.Clear();
                            Console.WriteLine("Задание №2");


                            Console.ReadKey();
                        }
                        break;

                    case "3":
                        {
                            Console.Clear();
                            Console.WriteLine();


                            Console.ReadKey();
                        }
                        break;

                    default:
                        Console.WriteLine("Выберите корректное задание!");
                        Thread.Sleep(3000);
                        break;
                }
            }
        }
    }
}

```


Task1
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp19.Utils
{
    public class Task1
    {
        public double X { get; }
        public double Y { get; }

        public Task1(double x, double y)
        {
            X = x;
            Y = y;
        }

        public bool IsInArea()
        {
            double parabolaY = 2 - X * X;
            return  Y >= 0 && Y <= parabolaY;
        }
    }
}

```
