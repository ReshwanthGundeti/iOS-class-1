# iOS-class-1

import UIKit

var greeting = "Hello, playground"

print("Hii",10,12.25)


//String interpolation

// "\()"

var name = "Resh"
print("My name is \(name)")

var grade = "A"
print("Hello, \(name) you got \(grade) grade in iOS course")

var age = 24
print("Hello, \(name) your \(age) years old and when it divided \(24/2)")
print("""
 Hello world,
      hhhdhdhhd,
      jdjdjdjd
 """)  //used to print bulk lines

//\r carriage return
print("Hello all,\rwelcome to  class")

print("Welcome to swift programming language")
print("spring2022")
print("*******")
print("Welcome to swift" ,  terminator: "$$")
print(1,2,3,4,5)
print(1,2,3,4,5, separator: "-")

let Hear : String = "Hello!"
print(Hear , "All")

------------------------------------------------------------------------------------------------------------
CLASS -2 
//
//  ViewController.swift
//  Helloapp2
//
//  Created by Gundeti,Reshwanth on 1/20/22.
//

import UIKit

class ViewController: UIViewController {

    @IBOutlet weak var nameoutlet: UITextField!
    
    
    @IBOutlet weak var gradetext: UITextField!
    
    @IBOutlet weak var Displaylabel: UILabel!
    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view.
        
        
        
        
    }

    @IBAction func buttonClicked(_ sender: UIButton) {
        //read the data from textbox and storeit ina variable
        
        var name = nameoutlet.text!
        var grade = gradetext.text!
        
        //Change the display label with this format. Hello, name!
        
        Displaylabel.text = "Hello, \(name)! your grade is \(grade)"
        
    }
    
}
<hr>
Class --3
------------------------------------------------------
//
//  ViewController.swift
//  VowelTester
//
//  Created by Gundeti,Reshwanth on 1/25/22.
//

import UIKit

class ViewController: UIViewController {

    @IBOutlet weak var Textoutlet: UITextField!
    
    @IBOutlet weak var Displaylabel: UILabel!
    
    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view.
    }

    @IBAction func ButtonClicked(_ sender: UIButton) {
        
        //Read the text
        var enteredText = Textoutlet.text!
        //Check
        if(enteredText.contains("a") ||
           enteredText.contains("e") || enteredText.contains("i") || enteredText.contains("o") ||
           enteredText.contains("u")){
            Displaylabel.text = "The text contains vowels"
        }
        
        else{
            Displaylabel.text = "There are no vowels"
        }
    }
    
}

playground
---------------------
import UIKit

var shoppingList = "The shopping list contains: "
var foodItems = "Cheese, Butter, Chocolate Spread"
var clothes = "Socks, T-shirts"

if clothes.hasPrefix("Socks") {
         print("The first item in clothes is socks")
}
else{
            print("socks is not the first item in clothes")
}


    print(foodItems.split(separator: ","))

    if clothes.contains(",") {
    print("Clothes contains more than one item")
    }else{
                print("Clothes contain only one item")
}

    foodItems[foodItems.startIndex..<foodItems.index(foodItems.endIndex,offsetBy: -7)]

shoppingList += foodItems[foodItems.index(foodItems.startIndex, offsetBy: 8)..<foodItems.endIndex]

 clothes.remove(at: clothes.firstIndex(of: "T")!)
clothes.remove(at: clothes.firstIndex(of: "-")!)
print("\(shoppingList), \(clothes)")
clothes.insert(contentsOf: ", Trousers", at: clothes.endIndex)


let password = "Demo@123"
    let confirmPassword = "Demo@123"

    if password == confirmPassword {
        print("Password matches")
    }else{
        print("Passwords doesn't matches")
}

  let currentYear = "2021"
var enteredYear = "2020"

if currentYear.elementsEqual(enteredYear) == true
{
    print("Entered year matches with current year")
}
else{
    print("Entered year does not match with current year")
}

   var vehiclePoweredBy = "Diesel"

 if vehiclePoweredBy != "Electricity" {
 print("Vehicle is not eco-friendly")
 }else{
 print("Vehicle is eco-friendly")
 }

 let nameGiven = "Anthony Martial"
var enteredName = "ANTHONY MARTIAL"

if nameGiven.lowercased() == enteredName.lowercased(){
print("Entered name and given name matches with each other")
}else{
print("Entered name does not matches with the given name")
}

















