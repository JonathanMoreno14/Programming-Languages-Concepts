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


func numbers(num: Int) -> Int{
    if num > 50 {
        print("The number is greater than 50")
        return num
    }else {
        print("The number is less than 50")
        return num
    }
}

numbers(num: 78)
//Prints The number is greater than 50



```

Booleans & Conditional Logic

```swift

//Boolean and Conditional Logic

var todayIsFriday = true

todayIsFriday = false

var todayIsSaturday: Bool = true


//  Or ||
if true == false || true == true{
    print("WTFish")
}

var hasDataFinishedDownloading: Bool = false

if !hasDataFinishedDownloading {
    print("Loading data...")
}

hasDataFinishedDownloading = true

if 2 == 2 {
    print("Should  see this")
}


//Equal to:  ==
//Not equal to: !=
//Greater than: >
//Greater than or equal to: >=
//Less than or equal to: <=
//Less than: <

var bankBalance = 400
var itemToBuy = 400

if bankBalance >= itemToBuy {
    print("purchased item")
}

if itemToBuy > bankBalance{
    print("Not enough funds to purchase the item")
}

if itemToBuy == bankBalance{
    print("Your funds are know at 0")
}

var bookTitle1 = "Harry Potter"
var bookTitle2 = "Harryy otter"

if bookTitle1 != bookTitle2{
    print("Need to fix spelling on the book title")
} else if bookTitle2.characters.count > 10 {
    print("find a new title for the book")
}
else {
    print("Both book titles match")
}


```

Contants & Logical Operators

```swift

//Logical NOT operator - unary prefix operator

let allowedEntry = false

if !allowedEntry{ //if allowedEntry != true
    print("Access Denied")
}


let entreredDoorCode = true
let passedRetinaScan = false
let personWithCode = true


if entreredDoorCode && passedRetinaScan || personWithCode{
    print("Welcome")
}else {
    print("Access Denied Again")
}


let hasDoorKey = false
let knowsOverridePassword = true

if hasDoorKey || knowsOverridePassword {
    print("Welcome")
}else{
    print("Access Denied")
}


```
Arrays

```swift

//Arrays

var employee1Salary = 45000.0
var employee2Salary = 54000.0
var employee3Salary = 100000.0
var employee4Salary = 20000.0



var employeeSalaries = [45000.0, 54000.0, 100000.0, 20000.0]
print(employeeSalaries.count)

employeeSalaries.append(3900.34)

print(employeeSalaries.count)

employeeSalaries.remove(at: 1)

print(employeeSalaries.count)


var students = [String]() //empty array of strings
print(students.count)

students.append("Jon")
students.append("Jacob")
students.append("Jose")
students.append("Smith")
students.append("Will")

print(students)



```

Loops

```swift


//Bad way
var employee1Salary = 45000.0
var employee2Salary = 100000.0
var employee3Salary = 54000.0
var employee4Salary = 20000.0


employee1Salary = employee1Salary + (employee1Salary * 0.10)



//A bit Better
var salaries = [45000.0, 100000.0, 54000.0, 20000.0]

salaries[0] = salaries[0] + (salaries[0] * 0.10)
salaries[1] = salaries[1] + (salaries[1] * 0.10)


//...
var index = 0
repeat {
  salaries[index] = salaries[index] + (salaries[index] * 0.10)
  index += 1
}while (index < salaries.count)




for  i in 0 ..< salaries.count {
    salaries[i] = salaries[i] + (salaries[i] * 0.10)
}

for salary in salaries {
    print("Salary:\(salary)")
}


```
Dictionaries

```swift

//Dictionaries

//Hash table 


var namesOfInteger = [Int: String]()

namesOfInteger[3] = "three"
namesOfInteger[44] = "forty four"

namesOfInteger = [:]


var airports: [String : String] = ["YYZ" : "Toronto Pearson", "LAX" : "Los Angeles International"]

print("The airports dictionary has: \(airports.count) items")

if airports.isEmpty{
    print("The airport dictionary is empty")
}

//change an update
airports["LHR"] = "London"
airports["LHR"] = "London Heathrow"
airports["DEV"] = "Dev Internationl"

//destroy and remove the iteme
airports["Dev"] = nil

for (airportsCode, airportName) in airports{
    print("\(airportsCode): \(airportName)")
}

for key in airports.keys{
print("Key ; \(key)")
}

for val in airports.values{
    print("Values : \(val)")
}

```

Optionals

```swift

//Optionals

var lotteryWinnings: Int?

//when ever you have a question mark make sure to use if let to check if its not nil


if lotteryWinnings != nil{
    print(lotteryWinnings!)
}

lotteryWinnings = 100

if let winnings = lotteryWinnings {
    print(winnings)
}

class Car {
    var model:String?
    
}

var vehicle: Car?

//if let v = vehicle{
//    if let m = v.model{
//        print(m)
//    }
//}

vehicle = Car()
vehicle?.model = "Bronco"

if let v = vehicle, let m = v.model{
    print(m)
}

var cars: [Car]?

cars = [Car] ()

if let caRR = cars , caRR.count > 0 {
    //only execute if not nil an if more 0 elements
}else {
    cars?.append(Car())
    print(cars?.count)
}

class Person {
     var _age: Int!
    
    var age:Int {
        if _age == nil{
            _age = 0
        }
        return _age
    }
    
    func setAge(newAge: Int){
        self._age = newAge
    }
}

var jack = Person()
//print(jack._age)
print(jack.age)


class Dog {
    var species: String
    
    init(someSpecies: String){
        self.species = someSpecies
    }
}

var lab = Dog(someSpecies: "Black Lab")
print(lab.species)



```
Object Oriented Programming

```swift

//Object Oritented Programming

class Vehicle {
    var tires = 4
    var headlights = 2
    var horsepower = 468
    var model = ""
    
    func drive(){
        //accelerate the vehicle
    }
    
    func brake(){
        
    }
}

let bmw = Vehicle()
bmw.model = "328i"

let ford = Vehicle()
ford.model = "F150"
ford.brake()

func someFunction(vehicle: Vehicle){
    vehicle.model = "Cheese"
}

print(ford.model)

someFunction(vehicle: ford) //Pass by reference
print(ford.model)

var someonesAge = 20

func passByValue (age: Int){
    let age = age
}

passByValue(age: someonesAge)


```
Inheritance

```swift



//Inheritance


class Vehicle {
    var tires = 4
    var make: String?
    var model: String?
    var currentSpeed: Double = 0
    
    init() {
       print("I am the parent")
    }

    
    func drive(speedIncrease: Double){
        
        currentSpeed += speedIncrease * 2
    }
    
    func brake(){
        
    }
    
}


class Truck: Vehicle{
    override init(){
        super.init()
        
    }
    
    override func drive(speedIncrease: Double) {
        currentSpeed += speedIncrease
    }

    
}

class SportsCar : Vehicle {
    
    override init(){
        super.init()
        print("I am the child")
        make = "BMW"
        model = "3 Series"
    }
    
    override func drive(speedIncrease: Double) {
        currentSpeed += speedIncrease * 3
    }
    
}

let car = SportsCar()

```
Polymorphism

```swift


```
