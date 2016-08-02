# Swfit 3

Variables & Operators

```swift
//: Playground - noun: a place where people can play

import UIKit

var str = "Hello, Playground"

//Operator
//Unary, Binary, Ternary

//Unary
var amICool = true
amICool = !amICool

//Binary
var message = "Hello Jonathan"

//Ternary
var feelGood= true
feelGood = amICool ? true : false

var bankAccntBalance = 100
var cashRegistermessage = bankAccntBalance >= 50 ? "You bought the item" : "You do not have enough funds"

```

Strings

```swift
//Strings
var age = 21
var firstName = "Jonathan"
var lastName = "Moreno"

var fullName = firstName + " " + lastName

//interpolation
var fullName2 = "\(firstName) \(lastName) is \(age)"

fullName.append(" II")


var bookTitle = "rework"
bookTitle = bookTitle.capitalized


var allCaps = "HELLO WORLD"
var lowCaps = allCaps.lowercased()


//removing certain words example: Heck, Fetch
var sentence = "What the fetch?! Heck that is crazy!?"

if sentence.contains("fetch") || sentence.contains("Heck"){
    sentence.replacingOccurrences(of: "fetch", with: "Douce")
    sentence.replacingOccurrences(of: "Heck", with: "Dang")
}

```

Numbers

```swift


```

Functions

```swift


```

Booleans & Conditional Logic

```swift


```

Contants & Logical Operators

```swift


```
Arrays

```swift


```

Loops

```swift


```
Dictionaries

```swift


```

Optionals

```swift


```
Object Oriented Programming

```swift


```
Inheritance

```swift


```
Polymorphism

```swift


```
