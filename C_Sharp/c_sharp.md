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



####Interface
```C#

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace C_Sharp
{         //Interfaces
  public interface info
 {
     void showInfo();

 }
 public class ProgramTwo : info
 {
     string name;
     int age;


     public ProgramTwo()
     {
         name = "";
         age = 23;
     }

     public ProgramTwo(string a , int b)
     {
         name = a;
         age = b;
     }

     public void showInfo()
     {
         Console.WriteLine("Name: {0}", name);
         Console.WriteLine("Age: {0}", age);

     }
 }

 class Program
 {
     static void Main(string[] args)
     {
         ProgramTwo info = new ProgramTwo("John", 23);
         info.showInfo();
         Console.ReadLine();
     }
 }
}
    /*
    Name: John
   Age: 23
   */


```

####Inheritance
```C#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace C_Sharp
{         //Inheritance
    class ProgramTwo
    {
        protected  string name;
        protected int age;
        public void getName(string nombre)
        {
            name = nombre;
        }
        public void getAge(int años)
        {
            age = años;
        }
    }
        class ProgramThree : ProgramTwo
        {
            public string getName()
            {
                return name;
            }

            public int getAge()
            {
                return age;
            }
        }


        class Program
        {
            static void Main(string[] args)
            {
                ProgramThree pt3 = new ProgramThree();
                pt3.getName("John");
                pt3.getAge(23);
                Console.WriteLine("Your name is: {0}", pt3.getName());
                Console.WriteLine("Your age is: {0}", pt3.getAge());
                Console.ReadLine();
            }
        }
    }

    /*
    Your name is: John
    Your age is: 23


    */

```


####Constructors
```C#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace C_Sharp
{         //Constructors
    class Program
    {
        string person;
        int idNumber;

        public Program()   
        {
            person = "John";
            idNumber = 10934;
        }

        public static void Main()
        {
            Program info = new Program(); 
            Console.WriteLine(info.person);
            Console.WriteLine(info.idNumber);
            Console.Read();
        }
    }
}

    /*
    John
    10934
    */



```

####Assessor
```C#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace C_Sharp
{         //Assessor
    class ProgramTwo
    {
        public string person;
        public string Person
        {
            get
            {
                return person;
            }
            set
            {
                person = value;
            }
        }
    }

    class Program 
    {

        public static void Main()
        {
            ProgramTwo pt2 = new ProgramTwo();
            pt2.person = "Jonathan";
            Console.WriteLine("My name is: {0}", pt2.person);
            Console.ReadLine();
        }
    }

}

        /*

        My name is: Jonathan

        */


```


####Methods
```C#

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Numbers
{          ///Method
            class Program
            {
            
                public static void numberGreater(int n)
            {
                if (n > 50)
                {
                    Console.WriteLine("The number is greater that 50");
                }
                else {
                    Console.WriteLine("The number is less than 50");
                }
            }
            
                static void Main(string[] args)
                {
                    Console.WriteLine("Enter a Number:");  //Enter the number
                    int num = Convert.ToInt32(Console.ReadLine());  //Converts string to interger from the number input
                    numberGreater(num);  //Calls method numberGreater(int n)
                    Console.WriteLine(num); //prints out the conditional statement result
                    Console.ReadLine();
                }
          }
}

/*
Enter a Number:
34
The number is less than 50
34


*/


```


####Properties
```C#

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace C_Sharp
{         //Properties
    class ProgramTwo
    {

        string name = "";
        int age = 0;
        int id = 0;
        public string Name
        {
            get
            {
                return name;
            }
            set
            {
                name = value;
            }
        }
        public int Age
        {
            get
            {
                return age;
            }
            set
            {
                age = value;
            }

        }
        public int ID
        {
            get
            {
                return id;
            }
            set
            {
                id = value;
            }
        }

        public override string ToString()
        {
            return "Name = " + Name + "  Age = " + Age + " ID " + ID ;
        }


        class Program
        {
            static void Main(string[] args)
            {
                ProgramTwo pt2 = new ProgramTwo();
                pt2.Name = "John Rambo";
                pt2.Age = 23;
                pt2.ID = 10123;
                Console.WriteLine("Identification - {0}", pt2);
                Console.ReadLine();
            }
        }
    }
}

/*

    Identification - Name = John Rambo  Age = 23 ID 10123

*/



```

####Loops

```C#


   ///for
  class Program
   {
      static void Main(string[] args) 
      {
          int num = 10;
            for (int i = 0; i < num; i++)

            Console.WriteLine(i);
            Console.ReadLine(); 
      }
   }
   /*
     0     1     2     3     4     5     6     7     8     9
  */



///while
class Program 
   {
      static void Main(string[] args) 
      {
        int num = 0;

            while (num < 10)
            {
                Console.WriteLine(num);
                num = num + 1;
            }
            Console.ReadLine(); 
      }
   }
  
  /*
     0     1     2     3     4     5     6     7     8     9
  */
  
  
  
  ///do while
class Program 
   {
      static void Main(string[] args) 
      {
            int num = 10;
            do
            {
                Console.WriteLine("value of num: {0}", num);
                num = num + 1;
            }
            while (num < 20);
            Console.ReadLine(); 
      }
   }

  /*
   value of num: 10   
   value of num: 11   
   value of num: 12   
   value of num: 13   
   value of num: 14   
   value of num: 15   
   value of num: 16   
   value of num: 17   
   value of num: 18   
   value of num: 19
  */
  
  
  
   ///foreach
  class Program
   {
      static void Main(string[] args) 
      {
       ArrayList listName = new ArrayList();
            listName.Add("John");
            listName.Add("Jonathan");
            listName.Add("Jim");

             foreach(string name in listName)
             Console.WriteLine(name);
             Console.ReadLine(); 
      }
   }
    /*
    John
    Jonathan
    Jim
    */
    
    

```

####Collections

```C#


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Collections;

namespace C_Sharp
          //Collections
{         //Arrays
        class Program
        {
            static void Main(string[] args)
            {
            int[] n = new int[5]; 
            int i, j;

          
            for (i = 0; i < 5; i++)
            {
                n[i] = i + 100;
            }

           
            for (j = 0; j < 5; j++)
            {
                Console.WriteLine("Element[{0}] = {1}", j, n[j]);
            }
            Console.ReadKey();
          
            }
        }
    }
/*

    Element[0] = 100
    Element[1] = 101
    Element[2] = 102
    Element[3] = 103
    Element[4] = 104

*/



    //Collections
    //List
  class Program
        {
            static void Main(string[] args)
            {
            List<int> list = new List<int>();
            list.Add(1);
            list.Add(2);
            list.Add(3);
            list.Add(4);
            list.Add(5);
            list.Add(6);

            foreach (int num in list) 
            {
                Console.WriteLine(num);
            }
            Console.ReadKey();
          
            }
        }
        /*
            1
            2
            3
            4
            5
            6
        */
        
        
        
        //Collections
        //Dictionaries
    class Program
        {
            static void Main(string[] args)
            {
            Dictionary<string, int> names = new Dictionary<string, int>();
            names.Add("John", 1);
            names.Add("Steve", 2);
            names.Add("Bill", 3);
            names.Add("Larry", 4);

            foreach (var pair in names)
            {
                Console.WriteLine("{0}, {1}",
                pair.Key,
                pair.Value);
            }
            Console.ReadKey();
          
            }
        }
    }

        /*
        John, 1
        Steve, 2
        Bill, 3
        Larry, 4
        */

```
