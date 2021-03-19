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


### **Enheritance**
***
   - **Wrapping up of Data Members and Member Functions**
   - Bundling data witth methods that can operate within a class
   
   > ***Essentially, It is the idea of **Hiding Data** within a class, preventing anything outside of class from directly interaction***
   
   - This does not means that members of another class cannot interact at all with the attribute of another obj
   
   - Membeers of other classes can interact with the attributes of another object through its methods

- **Methods**
| **Getters Methods** | **Setters Methods** |
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










