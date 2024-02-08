# *Keywords in Java*
## Access Modifiers
- public
- private
- protected

## Non Access Modifiers
- static
- final
- volatile
- transient
- abstract
- synchronized




## Miscellaneous
- strictfp
- import
- package 
- native
- enum
- void
- instanceof


## Flow Control
- if
- else
- while 
- for
- do 
- break
- continue
- return 
- switch
- default
- case



## Error Handling
- try 
- catch 
- throw 
- throws
- assert    
- finally

## OOP
- class
- implements
- extends
- interface
- new
- super 
- this

## Datatypes 
- <pre>byte      1 
- <pre>short     2
- <pre>int       4  
- <pre>long      8
- <pre>float     4
- <pre>double    8
- <pre>char      2
- <pre>Boolean   NA 
- JVM will provide the default values
 
## Un used categories
- goto
- const


## Implicit Conversions

- byte + byte = int
- string + int = string
- short + int = int
- byte + short = int

## Variable 
- global scope
- local scope
    - scope is inside block, method and Constructor
- instance
    - inside the class in any number of methods
- static

## Calling static Variable
- directly
- by using class name
- by using object Reference Variable

## Class vs Object
- <pre>characteristic of class
    - state
    - behaviour:
        represent behaviour of an object
    - Identity:
        used to identify object uniquely
- <pre>Calling Class
    - Declaration:
        ClassName ObjRefVar =
    - Instantanize:
        new keyword to allocate memory
    - Initialize:
        contructor initialization


___

# Some rules
 - cant use Instace variables in Static area (need to create object)
 - can use instance methods in  \<someone fill this shit>
 - A <strong>static method cannot access a class's instance variables and instance methods,</strong> because a static method can be called even when no objects of the class have been instantiated. For the same reason, the this reference cannot be used in a static method.

---

## Memory Allocation
-   <pre>Memory allocated during runtime
- Heap Memory(public Memory)
    - for objects
    - more memory requied
    - new keyword
        <pre>error thrown is "OUT OF MEMORY ERROR"
- Stack Memory(private Memory)
    - function call and local variable
    - less memory required
    - variable will be destroied when done using
        <pre>Error thrown by JVM "STACK OVERFLOW ERROR"

## Instance Methods

- Acessor - Getter Method
    - ```java
        class id{
                private id;
                public void getID(){
                    syso(id);
                }
        }
        ```
- Mutator Method - Setter method
     -<pre>Class id{
            private id;
            public void setID(int id){
                this.id = id;;
        }
    }

## Methods in Java
- <pre>methods are a way to organize code by grouping together a series of statements that perform a specific task
- Method Header:  Acess Specifier ReturnType Name   (ParameterList){
Method Signature
}

- Types of Methods
    - User Defined
    - Pre Defined
    - Abstract

- if method doesnt have a body it is called ABSTRAC

### FIVE Sense Organs of Java
---
- Methods
- Variables
- Constructors
- Instance Blocks
- Static Blocks















### static variables
- Static Variables: When a variable is declared as static, then a single copy of the variable is created and shared among all objects at a class level. Static variables are, essentially, global variables. All instances of the class share the same static variable.
- Important points for static variables :-
    - we can create static variables at class level only. See here
    - static block and static variables are executed in the order they are present in a program.
``` java
// Java program to demonstrate execution
// of static blocks and variables
class Test {
    // static variable
    static int a = m1();
   
    // static block
    static
    {
        System.out.println("Inside static block");
    }
   
    // static method
    static int m1()
    {
        System.out.println("from m1");
        return 20;
    }
   
    // static method(main !!)
    public static void main(String[] args)
    {
        System.out.println("Value of a : " + a);
        System.out.println("from main");
    }
}
```


### Non-Static Variable
- Local Variables: A variable defined within a block or method or constructor is called local variable.
- These variables are created when the block in entered or the function is called and destroyed after exiting from the block or when the call returns from the function.
- The scope of these variables exists only within the block in which the variable is declared. i.e. we can access this variable only within that block.
- Initialisation of Local Variable is Mandatory.
### instance variables
- Instance variables are non-static variables and are declared in a class outside any method, constructor or block.
    - As instance variables are declared in a class, these variables are created when an object of the class is created and destroyed when the object is destroyed.
    - Unlike local variables, we may use access specifiers for instance variables. If we do not specify any access specifier then the default access specifier will be used.
    - Initialisation of Instance Variable is not Mandatory. Its default value is 0
    - Instance Variable can be accessed only by creating objects.
### <a href="https://www.geeksforgeeks.org/difference-between-static-and-non-static-variables-in-java/">GFG article for static/instance/local var</a>
____


# Class vs Object
 - object is a instance of a class
















## instance methods 
- accessor method  - getter()
    ```java
    void setter(string name){
        this.name = name;
    }
    ```
- mutautor method - setter()
    ```java
    string getname(){
        return name;
    } 
    ```

____
____

## Heap Memory 
- used to store Objects
- out of memory error
- more memory 
- public memory 
- <strong>new</strong> is used 
## stack memory 
- function calls / initialize contructors
- local variables
- stack overflow error
- less memory
- private memory
- object will be destroyed when it becomes <strong>out of scope</strong>




## Method
- way to perfoem some tasks
- in java is a collction of instructions that collectively perform some task
- ```java
    
  public static int sum(int a, int b){ 
         return a + b; 
    }
    ```
- Method Header = public int sum(int a, int b)
- Method signature = sum(int a, int b)
<br>
<br>
    - {Access specifier} {return type} {method name} ( {params} ) 
    - {
        - method body
    - }

- Ramdom keywords:
    - Method overloading - parameter based
    - User defined methods
    - abstrct methods
    - static/instance methods 


## class structure
- data members (variables)
- methods 
- contructors
- static block
- instance block

## Constructors
- <pre>ClassName(){
        do something at the time of object creation
        defaultly it doesnt do anything
     }
- used for object creation or initialization
    - Dfault constructor i.e zero arguement  ClassName()
    - User defined parameterized constructor
    - can overload constructors based on params
    - 
    - No return type
```java
package LAB2;

public class constructor {
    public static class test{
        int a;
        int b;
        int c;

        test(){
            this.a = 0;
            this.b = 0;
            this.c = 0;
        }

        test(int a, int b, int c){
            this.a = a;
            this.b = b;
            this.c = c;
        }
        public void getter(){
            System.err.println(a+"===="+b+"===="+c);
        }
        public void addder(){
            System.err.println("addition="+(a+b+c));
        }
    }

    public static void main(String[] args) {
        test t0 = new test();       // default constructor
        t0.a=10;


        

        test t1= new test(10,3,10);     // user defined constructor
        t1.getter();
        t1.addder();
    }
}
    
```

___
### Conversion of Local variable to static variable and instance variable

```java
package thierory;

public class conversions {
    int a;
    static int static_a;

    void convert(int arg) {
        int local= arg+10;


        
        this.a=local;
        static_a=local;
    }

    public static void main(String[] args) {
        conversions t= new conversions();
        t.convert(10);
        
    }
}

```


## Array
- collection of same typed objects
- length fixed at the time of creation
- ```java
    int[] arr={1,24,5,6,7,7,7};
    int arr[]={24,12,5,15,1,5};
    //indices 0 1 2 3 ...n-1 for a array of length n
    for(int i=0; i<arr.length ; i++){
        System.out.println(arr[i] + " ");
    }

  ```





___

### Final Keyword:
- non-access modifier
- used for classes , attributes/variables and methods
- makes them non-changeable (cannot inherit or override)
- final keyword used when want to store the same value like pi = 3.1415
- called <i>"Modifier"</i>
    - Stop values change
    - Stope method overloading
    - stop inheritance



#### final Variable
```java
class Bike{
    final int speedlimit=90; // final variable
    void run(){
        speedlimit=140;    
    }

    public static void main(String args[]){
        Bike b= new Bike();
        b.run();
    }
}
```


```bash
Output :  Compile time error
```





#### final method
```java
class Bike{
    final void run(){
        System.out.println("final running"); 
    }
}

   
class Honda extends Bike{

    void run(){
        System.out.println("honda bike running overloading....");
    }
    
    public static void main(String args[]){
        Honda h= new Honda();
        honda.run();
    }

}     

```


```bash
Output :  Compile time error
```






#### final class
(cannot extend final class)
```java
final class Bike{
    
}

   
class Honda extends Bike{

    void run(){
        System.out.println("honda bike extending....");
    }
    
    public static void main(String args[]){
        Honda h= new Honda();
        honda.run();
    }

}     

```


```bash
Output :  Compile time error
```





_____

## Method
- method have a return type constructor dont.

### Overloading
1. Based on number of arguments
2. Based on data type
 

### Overriding
- occurs when a child class has its method implementation for the method already present in the parent class















































