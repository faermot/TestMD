<img src="https://github.com/user-attachments/assets/f57852aa-b866-4a98-b1f2-5788c74bcd49" width="135" />
```C#
using ConsoleApp5.UtilsTask;
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading;
using System.Threading.Tasks;

namespace ConsoleApp5
{

    internal class Program
    {
        static void Main(string[] args)
        {
            while (true)
            {
                Console.Clear();
                Console.Write("Выберите задание: ");
                switch (Console.ReadLine())
                {
                    case "1":
                        Console.Clear();
                        Console.WriteLine("Задание 1");

                        TaskPerson person = new TaskPerson("Андрей", 3);
                        person.Print();

                        Thread.Sleep(4000);
                        break;

                    case "2":
                        Console.Clear();
                        Console.WriteLine("Задание 2");
                        

                        TaskCar car = new TaskCar("Audi", "Q7", 2020);
                        car.Print();

                        Thread.Sleep(4000);
                        break;

                    case "3":
                        Console.Clear();
                        Console.WriteLine("Задание 3");

                        TaskBook book = new TaskBook("Носы", "Альберт Гадунов", 188);
                        book.Print();



                        Thread.Sleep(4000);
                        break;

                    case "4":
                        Console.Clear();
                        Console.WriteLine("Задание 4");

                        TaskRectangle rectangle = new TaskRectangle(27, 61);

                        rectangle.Width = 27;

                        rectangle.Print();  
                        rectangle.Calculate();

                        Thread.Sleep(4000);

                        break;

                    case "5":
                        Console.Clear();
                        Console.WriteLine("Задание 5");

                        TaskCircle circle = new TaskCircle(10);

                        circle.Print();
                        circle.Calculate();

                        Thread.Sleep(4000);
                        break;

                    case "6":
                        Console.Clear();
                        Console.WriteLine("Задание 6");

                        TaskStudent student = new TaskStudent("Андрей", "C", 13);
                        student.Print();

                        Thread.Sleep(4000);
                        break;
                    case "7":
                        Console.Clear();
                        Console.WriteLine("Задание 7");




                        Thread.Sleep(4000);
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
