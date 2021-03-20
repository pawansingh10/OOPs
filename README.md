# OOPs


## Introduction to Object Oriented Programming
**
- In order to understand **OOPs**, first understand **Objects**
- In order to understand **Objects** first  understand **Primitive Data Type**

### **Primitive Data Types**
***
- Variable that stores single, simple values
- Example
  - **Byte**
  - **char**
  - **boolean**
  - **Int**
  - **Float**
  - **double**
  
- When program is small & so simple programmers uses Primitive Data types However As programs became Large & Complex Primitive Data tpes is not sufficient

- So Programmers start using the group of Primitive data types

- **Structure & Array**
- | Structures | Arrays |
  |------------|---------|
  | Stores groups of data | Stores groups of data|
  | Can store different types of data | Can store only similar types of data| 
  | Heterogeneous | Homogeneous|
  | store int, char, bool or even another struct |stores only similar data types|

### Issues with Structures
***
- The main problem with structure is that you **Cannot define functions** within a structure

- In the world of OOPs, **Objects allows us to store data of different kind together along with Funtions additionally**


### **Objects**
***
  - **Objects** are instances of a **class**
  - **Classes** are templates for an **Objects**
  
- ```code
     class Human:
          name ;
          age ;
          //Not initialize the instance variable because for different obj its value is different
          eat();
          speak();
          move();
          // methods are same for every obj that's why it's is define within class
  ```
  
> **OOPs hepls programmers to create complex programs by grouping related Data and Functions together**
- Data_1, Function1, Data_2, Function2, Function3, Data_3 etc
- | data | Function|
  |------|---------|

## **4 Main Principles of OOPs**
***
* **1. Encapsulation**
* **2. Abstraction**
* **3. Polymorphism**
* **4. Inheritance**


### **Encapsulation**
***
   - **Wrapping up of Data Members and Member Functions**
   - Bundling data witth methods that can operate within a class
   
   > ***Essentially, It is the idea of **Hiding Data** within a class, preventing anything outside of class from directly interaction***
   
   - This does not means that members of another class cannot interact at all with the attribute of another obj
   
   - Membeers of other classes can interact with the attributes of another object through its methods

- **Methods**
- | **Getters Methods** | **Setters Methods** |
  |---------------------|---------------------|
  | For retrieving information | For setting & changing information |

- ```code
     h1.getName();
     // check the name of any object of Human class anywhere in this program

- In case of you want to some attributes to be **Read only** from the outside
  - For this, you would **define a getter method** not a setter method
  - The variable could only be referenced, not changed


- **Encapsulation - Information Hiding**
  - Genreally best to not allow external classes to directly edit an object's attributes
  - This is very important when working on large and complex programs
  - Each piece should not have access to to rely on the inner working of other sections of code
  
  - **Information Hidding**, or keeping the data of one class hidden from external classes, helps you **keep control of your program** and **prevent it from becoming too complicated**

### Why Encapsulation?
***
- Encapsulation is the important principle of OOPs
  - Keeps the programmer in **control of Access to data**
  - Prevents the program from ending up in any **Unwanted states**


### **Abstraction**
***
   - **Only Showing Essesntial Details & Keep everything else hidden**
   
- **Car Example**
   - |**Essesntial Details**|
     |----------------------|
     | How the steering wheel steers the car|
     |How much fuel car have|
     | How breaks works |
     | How much car speed|


- It extends to OOPs

- The Classes you create should act like yyour car, **Users of your Classes should not worry about the inner details of those classes**

- Classes should not directly interact with other classes data 

- Abstraction is very inportant when you working on your program incrementlly
- | Section-1 | -> | Section-2 | -> | Section-3 |
  |-----------|----|-----------|----|-----------|
  
- Modern programs are very complex to the point where **multiple programmers tends to work on one program**
- In this case, It is the best if the section that you work on is able to to function without knowledge of inner working of your colleague's's section


### Abstraction - Interface and Implementation
***
- **Interface**
  - Interface refers to way section of code **can communicate with one another**
  - This typically is done through methods that each class is able to access
  
- **Implementation**
  - The inplementation of these methods, or how these methods are coded,should be hidden
  - Not accessible outside the class
  - How is not important, work or not is important
  
- If Classes are entangled then one change creates a ripple effect that cause many more changes

- **Creating an Interface through which classes can interact ensure that each piece can individually developed**

#### Abstraction allows the program to be worked on incrementally and prevent it from becoming complex and entangled


### **Inheritance**
***
   - Inheritance is the principle that allows classes to derive from other class
- **Class Weapon**
   - This class contains common attributes and methods to all weapons
   - weapon.damage() 
   - weapon.attack()
   - Class sword
   - Class Gun
   - These two classes are different from one another
   
- | Super Class|
  |------------|
  | Sub class | sub class |
  |-----------|-----------|
  
- Class Hierarchy
   - You can create many more layer with many more classes in each layer
   
- **Access Modifiers**
   - Access Modifiers changes which class have access to other classes, methods or attributes
   - Three main Access Modifiers :- 
   - **1. Public**
   - **2. Private**
   - **3. Proctected**

* **Public**
   - **Public Members** can be access from anywhere in your program
   
   - This includes anywhere both inside of the class hierarchy as well as outside in the rest of program

   - |      |      |     Food |      |      |
     |------|----------|------|------|------|
     |      | Fruit|         | Vegetable|  | 
     |Mango |  | Apple |   Broccoli| 

* **Private**
   - **Private Member** can only access from within the same class that the member is defined
   - This allows us to create other multiple private members of the same class in different location so that they do not conflict  with another one
   
* **Proctected**
   - **Proctected Member** can be access within the class it is defined as well as any Subclass of that class
   - This essentially makes proctected members private to the hierarchy in which they are defined



### **Polymorphism**
***
   - Polymorphism describes the **methods that are able to take amny forms**
   - There are two types of polymorphism
   - **1. Dynamic/Runtime Polymorphism**
   - **2. Static/Compiletime Polymorphism**

* **Dynamic Polymorphism**
  - Occurs during **Runtime of program** when the program being executed
  - Runtime Polymorphism describe when a method signature is in both
  - The methods share the **Same name but have different implementation**
  - The implementation of the Subclass Override Superclass
  - ```code
       class Car:
           drive(miles){
               car.gas -= 0.04 * miles;
           }
           
       
       class sportsCar:
            drive(miles){
               sportscar.gas -= 0.02 * miles;
            }
            
          
        mySportsCar.drive(100);
        // This sportsCar drive() method overrride the Superclass drive() method
        myCar.drive(100);
        // While car drive() method same as it is
    ```
    
   - This works because of the form of the method is decided based on where in the class hierarchy it is called
   
   - The main benefits of the Dynamic polymorphism is that it allows us to write methods in the Superclass without having to include if or else if which subclass is used when a method is called.
   - 
   - The implementation of a method signature that will be used in **determined dynamically as the program is run**  


* **Static Polymorphism**
  - occurs during **compile time** rather than runtime
  - This refers to when **multiple methods with the same name but different arguments** are defined in the same class
  
- Way to differentiate methods of the same name

- Differents numbers of parameters
  - **Different types of parameters**
  - **Differents orders of parameters**

- ```code
       class car:
           
           drive(int speed, string destination)
           
           drive(int speed, int distance)
           
           drive(string destination, int speed)
           
  ```
 
- Method Overloading can cause trouble if you do not keep straight which parameters you need for which implementation
- Using the incorrect arguments may not cause an error if it matches that of another form of the method, which can cause issues

- Overall Polymorphism allows methods to take on many different forms
- When utilizing polymorphism and method overloading, be sure that you are calling the correct form of the method 
