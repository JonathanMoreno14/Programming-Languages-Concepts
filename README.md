# Programming-Languages-Concepts
This is a list of object oriented  programming languages that includes their syntax. The list can be used as a reference for the language.


Examples:

Finding out if the given number is greater than or less than 50.

#####Java
```java

public class numbers{
public static void num(int in){        // Method with parameter for integer
	    
    if(in > 50){         //Checks the conditional statement if in is greater than 50
        System.out.println("The number is greater that 50");   //if true prints this line
    }else{               //else prints this line
        System.out.println("The number is less than 50");
    }
}
public static void main(String[] args) {
     System.out.println("hello world");
     num(78);         //Method num(); 
   }

}

//Prints Hello World
//The number is greater that 50

```


#####Ruby
```ruby
def num(int= '')                     # Method def 
  if int > 50                        # The user inputs a number in num() it checks if the number is greater than 50
    "The number is greater than 50"
  else                               # else the number is less than 50 
    "The number is less than 50"
  end
end


 num(78) 
 #Prints The number is greater than 50

```

#####Javascript
```javascript
function numbers(nums){    //Function contains a nums within its parameters
    if(nums > 50){         //Checks conditional statement if nums is greater than 50
        console.log("This number is greater than 50"); //if so, then the console output prints this message
    }else{
         console.log("This number is less than 50"); //else it prints this console output
    }
}

numbers(78) 
//Prints This number is greater than 50

```
