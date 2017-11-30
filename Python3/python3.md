
# Python 3


### Keywords

```python

False	class	finally	is	      return
None	    continue	for	     lambda	 try
True	    def	     from	     nonlocal	 while
and	    del	     global	not	      with
as	    elif	     if	     or	      yield
assert   else	     import	pass	 
break   except      in	     raise	 

```



### Strings and Variables

```python

my_text = "We made it!"
print(my_text)

my_text = len("We made it!")
print(my_text)


```

### Numbers and math functions

```python
import math



i = 225
f = 12.5

a =25
b = 3
print(a + b)
print(a - b)
print(a * b)
print(a / b)

print(a ** b) #raised power 25^3
print(a // b)
print(a * b) #remainder operator

print(pow(2,3))
print(max(3,9,4,5,6))
print(min(3,9,4,5,6))

print(math.ceil(23.53))
print(math.floor(12.58))
print(math.sqrt(16))
print(math.sin(45))


```


### List

```python

food = ["pancake", "ramen", "pho"]

print(food[0])
print(food[1])
print(food[2])

food[1] = "noodle"
print(food)


meals = list()
print(meals)

customer = list(["leo", "john", "leo"])
print(customer)

numbers = [4,6,2,9,3]

print(5 in numbers)
print(4 in numbers)
print(4 not in numbers)


print(len(numbers))
print(min(numbers))
print(max(numbers))
print(sum(numbers))

print(numbers)

numbers.sort()
print(numbers)

numbers.reverse()
print(numbers)

numbers.append(7)
print(numbers)

new_list = [6,8]
numbers.extend(new_list)
print(numbers)


```


#### Dictionaires


```python

contacts = {
     'leo' : 'leo@email.com',
      'jeo' : 'jeo@email.com',
       'smith' : 'smith@email.com'
}

print(contacts)

print(contacts['jeo'])

contacts['tony'] = 'tony@email.com'
print(contacts)

del contacts['leo']
print(contacts)

print('leo' in contacts.keys())
print('tony' in contacts.keys())


contacts = {

     'leo':{
            'email': 'leo@email.com',
             'mobile': '12345678'
         },
      'jeo': {
             'email': 'jeo@email.com',
              'mobile': '12345645'
          },
     'smith': {
             'email': 'smith@email.com',
             'mobile': '12345234'
            }
}

print(contacts['leo']['email'])
print(contacts['leo']['mobile'])



```

### Control flow

```python

i = 10
if i % 2 == 0:
    if i > 10:
        print("Number is even and greater than 10")
    elif i < 10:
        print("Number is even and less than 10")
    else:
         print("Number is even being 10")
else:
    print("Number is odd")


names = ["leo", "smith", "jason"]

for n in names:
    print(n)

index = 0
while index < len(names):
    print(names[index])
    index += 1


```


### Functions

```python

def say_hi(name, age):
    print("My names is " + name)
    print("I'm " + str(age) + " years old.")

say_hi("Adam", 27)
say_hi("Lee", 28)
say_hi("John", 29)


number = 15 #gloa

def summary():
    number = 20 #local variable
    global number2
    number2 = 25
    print("Inside: " + str(number))

summary()
print("Outside: " + str(number2))




```

### Classes

```python

class Restaurant:
   def _init_(self, name, address, revenue):
      self.name = name
      self.address = address
      self.revenue = revenue

      def show_address(self):
          print(self.address)

      def show_revenue(self):
          print(self.revenue)

      def order(self, money):
         self.revenue += money


```

### Modules

```python

n = math.sqrt(16)
print(n)

import my_module

print(my_module.number_of_styles)

text = "I love to Code"
print(my_module.style_upper(text))
print(my_module.style_lower(text))


```
