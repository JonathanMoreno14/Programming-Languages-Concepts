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

//Numbers
//Type interence
var age = 30
//Explicity declared type
var weight: Int = 200  //Int

var someNum: Double = 123423455455653

var mileRan = 56.45

var pi: Float = 3.14

//Arithemtic Operators
var area = 2 * 20

var sum = 2 + 20

var diff = 20 - 2

var div =  20 / 2

var remainder =  12 % 5


var randonNum  = 12

if randonNum % 2 == 0 {
    print("this is a even number")
}else{
    print("this is an odd number")
}


var orderOfOperations = 15 * ((5 + 7) / 3 )


```

Functions

```swift

//Functions

//DRY

//Shape1
var length = 5
var width = 10

var area = length * width

//Shape 2
var length2 = 6
var width2 = 12

var area2 = length2 * width2

//Shape 3
var length3 = 3
var width3 = 8

var area3 = length3 * width3



//Examples of a Function
func calculateArea(length: Int, width: Int) -> Int{
    let area = length * width
    return area
}
let shape1 = calculateArea(length: 5, width: 10)
let shape2 = calculateArea(length: 6, width: 12)
let shape3 = calculateArea(length: 3, width: 8)



var bankAcctBalance = 500.00
var itemPurchase = 350.00

func purchaseItem(currtBalance: Double, itemPrice: Double) -> Double{
    if itemPrice <= currtBalance{
        print("Purchased item for : $ \(itemPrice)")
        return currtBalance - itemPrice
    }else{
       print("You do not have enough funds to purchase item")
       return currtBalance
    }
}

bankAcctBalance = purchaseItem(currtBalance: bankAcctBalance, itemPrice: itemPurchase)

var itemPurchased = 40.00

bankAcctBalance = purchaseItem(currtBalance: bankAcctBalance, itemPrice: itemPurchased)


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
