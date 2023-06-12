# Inheritance

## Aim:
To write a C# program to print some messages using hierarchical inheritance.

## Algorithm:
### step 1:
Create a base class.
### step 2:
Create two child class.
### step 3:
Create a constructor in the base class and print a message.
### step 4:
create a function in child class to print a message.
## Program:
```
NAME : JANANI R
REGISTER NUMBER : 21221230039
```
```
using System;
namespace Vehicle
{
    public class tyre
    {
        public tyre()
        {
            Console.WriteLine("base class tyre");
        }
        public virtual void Display()
        {
            Console.WriteLine("tyre");
        }

    }
    public class scooter : tyre
    {
        public scooter()
        {
            Console.WriteLine("child class Scooter");
        }
        public override void Display()
        {
            base.Display();
            Console.WriteLine("scooter");
        }

    }
    public class car : tyre
    {
        public car()
        {
            Console.WriteLine("child class car");
        }
        public override void Display()
        {
            base.Display();
            Console.WriteLine("car");
        }
    }
    
    public class Program
    {
        static void Main(string[] args)
        {
            car cr = new car();
            scooter sc = new scooter();
            cr.Display();
            sc.Display();

        }
    }


}
```
## Output:
![EXP8](https://github.com/Janani-2003/Inheritance/assets/94288340/4e0b213e-6215-4d74-96a8-bd150b418d18)

## Result
Thus C# program to print some messages using hierarchical inheritance is written and executed sucessfully.
