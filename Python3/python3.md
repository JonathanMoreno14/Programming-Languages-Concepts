
# Python 3


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



```python






```



```python






```
