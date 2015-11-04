#C Sharp


####Encapsulation/Abstraction 

```C#

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace C_Sharp
{       //Encapsulation/Abstraction 

    class ProgramTwo
    {
        public double num1;
        public double num2;


        public  double getAdd() ///Add
        {
            return num1 + num2; 
        }
        public double getSub() ///Subtract
        {
            return num1 - num2;
        }
        public double getMul() ///Multiply
        {
            return num1 * num2;
        }
        public double getDiv() ///Divide
        {
            return num1 / num2;
        }

        public void Answers()
        {
            Console.WriteLine("Addition: {0}", getAdd());
            Console.WriteLine("Subtraction: {0}", getSub());
            Console.WriteLine("Multiplication: {0}", getMul());
            Console.WriteLine("Division: {0}", getDiv());
        }
    }


    class Program
    {
        static void Main(string[] args)
        {
            ProgramTwo pt = new ProgramTwo();
            pt.num1 = 14;
            pt.num2 = 9;
            pt.Answers();
            Console.ReadLine();
        }
    }

    /*
      Addition: 23
      Subtraction: 5
      Multiplication: 126
      Division: 1.55555555555556

    */
}

```

####Polymorphism


```C#

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace C_Sharp
{       //Polymorphism

    class ProgramTwo
    {
        public void display(string name)
        {
            Console.WriteLine("Your name is : " + name);
        }
        public void display(int age)
        {
            Console.WriteLine("Your Age is : " + age);
        }
        public void displayNumber(long number)
        {
            Console.WriteLine("Your Phone Number is : " + number);
        }
    }


    class Program
    {
        static void Main(string[] args)
        {
            ProgramTwo pt = new ProgramTwo();
            pt.display("John");
            pt.display(34);
            pt.displayNumber(8175551234);
            Console.ReadLine();
        }
    }

    /*
     Your name is : John
     Your Age is : 34
     Your Phone Number is : 8175551234

    */
}


```
