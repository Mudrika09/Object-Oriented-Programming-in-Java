# Object-Oriented-Programming-in-Java

**JAVA IS A PLATFORM-INDEPENDENT LANGUAGE**

The codes written in Java are converted into an intermediate level language called **bytecode**,after compilation which becomes a part of the java platform,independent of the machine on which the code runs.This makes Java highly portable as its bytecodes can be run on any machine by an interpreter called **Java Virtual Machine(JVM)**

**JAVA IDENTIFIERS**

An identifier can be a method name,class name,variable name or label.

**Code1:: FirstProgramme.java:** 

In this Code,there are 5 identifiers:

**FirstProgramme:** Class Name

**main:** Method name

**String:** predefined class name

**args:** variable name

**a:** variable name

**JAVA RESERVED WORDS**

There are **53** reserved words in Java of which **50** are **keywords** and **3** are **literals**(**true,false,null**)

# OOP CONCEPTS:

**CLASS:**

A class is a user defined blueprint or prototype from which objects are created.  It represents the set of properties or methods that are common to all objects of one type. In general, class declarations can include these components, in order:

    Modifiers : A class can be public or has default access.
    
    Class name: The name should begin with a initial letter (capitalized by convention).
    
    Superclass(if any): The name of the class’s parent (superclass), if any, preceded by the keyword extends. A class can only extend (subclass) one parent.
    
    Interfaces(if any): A comma-separated list of interfaces implemented by the class, if any, preceded by the keyword implements. A class can implement more than one interface.
    
    Body: The class body surrounded by braces, { }.

**OBJECT:** 

An object is an instance of a class.Technically, Class is a template which describes what state and behavior of an instance this class can have. Object implements the state and behavior in the form of variables and methods and requires some memory allocated.An object consists of:

    State : It is represented by attributes of an object. It also reflects the properties of an object.
    
    Behavior : It is represented by methods of an object. It also reflects the response of an object with other objects.
    
    Identity : It gives a unique name to an object and enables one object to interact with other objects.
    
    
**Declaring Objects (Also called instantiating a class):**

When an object of a class is created, the class is said to be **instantiated**. All the instances share the attributes and the behavior of the class. But the values of those attributes, i.e. the state are unique for each object. A single class may have any number of instances.


**CONSTRUCTORS:**

Constructors are used for initializing new objects. Constructors does not return any values but implicitly it returns the object of the class. Fields are variables that provides the state of the class and its objects, and methods are used to implement the behavior of the class and its objects.


**CONSTRUCTORS VS METHODS:**

Constructors in Java can be seen as Methods in a Class. But there is a big difference between Constructors and Methods.

1.Constructors have only one purpose, to create an Instance of a Class. This instantiation includes memory allocation and member initialization (Optional).

By contrast, Methods cannot be used to create an Instance of a Class.

2.Constructors cannot have Non Access Modifiers while Methods can.

3.Constructors cannot have a return type(Including void) while Methods require it.

4.The Constructor name must be the same as the Class name while Methods are not restricted.

5.As per Java naming convention, Method names should be camelcase while Constructor names should start with capital letter.

**JAVA ACCESS MODIFIERS:**

|           | **PRIVATE**|**DEFAULT**|**PROTECTED**|**PUBLIC**|
|:---------:|:----------:|:---------:|:-----------:|:--------:|
|**WITHIN SAME CLASS**|YES|YES|YES|YES|
|**FROM ANY CLASS IN SAME PACKAGE**|NO|YES|YES|YES|
|**FROM ANY SUB CLASS IN SAME PACKAGE**|NO|YES|YES|YES|
|**FROM ANY NON-SUB CLASS IN SAME PACKAGE**|NO|YES|YES|YES|
|**FROM ANY SUB-CLASS FROM DIFFERENT PACKAGE**|NO|NO|YES|YES|
|**FROM ANY NON-SUB CLASS FROM DIFFERENT PACKAGE**|NO|NO|NO|YES|



**FOLDER:Class and objects:**

**Code1:CreatingObjects1.java:** Shows the creation of object using 'new' keyword.The new operator instantiates a class by allocating memory for a new object and returning a reference to that memory.

**Code2:Constructor.java :** Shows the creation and invoking of a constructor.The new operator also invokes the class constructor.

**Code3:CreatingObjects2.java:** Shows the creation of object and accessing class members without creating a constructor.

**Code4:GuessingGame.java:** A simple game implemented using classes and objects.

**Code5:OrderOfExecution.java:** Shows the order of execution of static anonymous and init(constructor) block.From the output of this code it can be seen that STATIC block will execute only once when class gets loaded.But Anonymous block and Constructor will run every time object of a Class gets created. Init block will get executed first and then constructor.

**Code6:SwapObjects.java:** code to swap two objects of the same class with only one class member.

**Code7:SwapObjects2problem.java:** Code shows the problem to swap two objects of a class with more than one class members if we use the same way used in Code6.

**Code8:SwapObjects2Solution.java:** Code shows the solution to Code7 problem using Wrapper class.A wrapper class solution works even if the user class doesn’t have access to members of the class whose objects are to be swapped.


