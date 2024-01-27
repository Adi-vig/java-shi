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
    -<pre>Class id{
            private id;
            public void getID(){
                syso(id);
        }
    }
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
