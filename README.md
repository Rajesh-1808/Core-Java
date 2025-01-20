# Core-Java
Java notes


CORE JAVA INTORDUCTION:-
=========================
Why we need to learn JFS..?
=============================
-->To Develop the Applications.
-->Application means, it is a "Collection of Programs" , which can:
    -Take the request
    -Process the request
    -Send the response to the end user.
 ->There are 3 types of Applications:
    1)Desktop Applications(notepad,word, calculator,...)
    2)Web Based Applications(Facebook, Whatsapp, SBI,HDFC,...)
    3)Mobile Applications(notepad, Facebook)
---------------------------------------------------------------------------------------------------------------------------------------------------------------
Where we can use all these Concepts..?(Java, FET or UI, SQL)
=============================================================
-->In Generic, For Each and Every Application we have "4" layers:

 ->user -->Request   -->Response --> end user.
                |   |
                |   |
    1)View layer or presentation Layer(FET or UI):
        -->Taking the request from the end user, and creating web pages like home page, login page, error page, signup page, etc...
                |   |
                |   |
    2)Controller Layer(J2SE, J2EE, Frameworks):
        -->Performing the Validations and Business logics based on requirements.
        -->Processing the request
                |   |
                |   |
    3)Data Access Layer(JDBC or Hibernate):
       -->Translates the Java Technologies in to Database understandable Language and vice versa.
                |   |
                |   |
    4)Data Layer(SQL : MySQL or Oracle)
        ->Database, it is going to store the data and manipulate the data based of CRUD Operations.
---------------------------------------------------------------------------------------------------------------------------------------------------------------
Definition of Java or What is Java:-
=====================================
-->java is a simple , High-level, secure, platform independent, Robust and Object oriented programming language used for developing Both Standalone and Web(internet) Applications.
-->java is case sensitive programming language.
Note: Not a pure object-oriented language because it supports primitive data types like int, char etc.
---------------------------------------------------------------------------------------------------------------------------------------------------------------
WHY JAVA..?:-
============
-->Java Programming language is Invented for Developing Internet Applications by providing Platform independence(Write once run anywhere).
-->Java is one of the most popular programming language in the world.
-->Java is popular programming language for client-server web applications.
-->It has more demand in the current job market.
-->it is easy to learn and simple to use.
---------------------------------------------------------------------------------------------------------------------------------------------------------------
HISTORY OF JAVA:-
=================
-->Java history was started with the Green Team.
-->The Green Team started a project to develop a language for digital devices such as Television.
-->It works on Internet Programming.
---------------------------------------------------------------------------------------------------------------------------------------------------------------
CREATION OF JAVA:-
==================
-->Java was developed by James Gosling and his team (Mike shredding, park Naughton) at "Sun Microsystems INC" in the year 1991.
-->James Gosling is also known as Father of the java.
-->Initially, James Gosling call it as "Green Talk" with the file extension as ".gt"
-->Later on it is renamed as "OAK" and again it is renamed as "java" in the year 1995 , because "oak" is already a trademark by the "oak Technologies".
-->"java is a island in Indonesia where a first coffee was produced."
---------------------------------------------------------------------------------------------------------------------------------------------------------------
Java Divided into Three Categories:-
-------------------------------------
J2SE(java 2 standard Edition): For creating desktop-based applications.(Core java)
J2EE(java 2 Enterprise Edition) : For Creating enterprise web-based applications.(Adv Java)
J2ME(java 2 Micro Edition): For Developing mobile-based applications.(Frameworks)
---------------------------------------------------------------------------------------------------------------------------------------------------------------
JDK:- Java Development kit(JDK) is a software development kit required to develop applications in java. When you download JDK, JRE is also downloaded with it.
JRE:- Java Runtime Environment(JRE) is a software Package that provides java class libraries, JVM and other components that are needed to run java programs.
JVM:- Java Virtual Machine(JVM) is an interpreter that converts byte code into machine level language code .
===============================================================================================================================================================
Java version History:-
------------------------
1)JDk alpha and beta 
2)JDk 1.0
3)JDK 1.1
4)J2SE 1.2
5)J2SE 1.3
6)J2SE 1.4
7)J2SE 5(1.5)
8)Java SE 6(1.6)
8)Java SE 7(1.7)
9)Java SE 8(1.8)
10)Java SE 9(1.9)
11)Java SE 10(1.10)
12)Java SE 11
13)Java SE 12
14)Java SE 13
15)Java SE 14
16)Java SE 15
17)Java SE 16
18)Java SE 17
19)Java SE 18
20)Java SE 19
21)Java SE 20
22)Java SE 21
23)Java SE 22
24)Java SE 23
25)Java SE 24
26)Java SE 25

latest version: JAVA SE 23
Feature Updates: JAVA SE 24, 25
old version and under maintainance:- (JAVA SE 8, JAVA SE 11, JAVA SE 17, JAVA SE 21)
(Alpha & beta, 1.0, 1.1, 1.2, 1.3,1.4,1.5, 1.6, 1.7,1.9,1.10, 12, 13, 14, 15, 16, 18, 19, 20) -->Old version not in maintenance.
================================================================================================================================================================
JAVA PROGRAM STEP BY STEP EXECUTION PROCESS:-
===============================================
-->Step-1:  create a java source code file with .java extension
-->step-2:  compile the source code using the java compiler which will creates a bytecode file with .class extension.
-->Step-3:  class loader reads both user defined and library classes into memory for execution.
-->step-4:  bytecode verifier validates all the byte codes are valid.
-->step-5:  JVM(java virtual machine) reads bytecodes and translate into machine Level Language for execution. 
================================================================================================================================================================
JVM ARCHITECTURE:-
===========================
Why do we need JVM:-
--------------------
-->Operating System is not provided environment to execute java Applications or programs.
-->To execute java programs or Applications we must need  to have JVM.
----------------------------------------------------------------------------------------------------------------------------------------------------------------
what is JVM? -->JVM is a interpreter which is responsible for loading, verifying and executing byte code created in java.
-->".Class" file is the input to the JVM.
ARCHITECTURE:-
--------------
".class"--> 1)Class Loader Subsystem:
                 -->Loading(Classes will be loaded by this Component)
                      -->Bootstrap Class Loader -->Responsible for loading classes from BootStrap class path, Nothing but rt.jar(contins all of the compiled 
                         class files)
                      -->Extension Class Loader-->Responsible for loading Classes find in the ext.folder("/jre/lib").
                         -->From java 9 , we can call "Extension class Loader" as "Platform Class Loader."
                      -->Application Class Loader -->Responsible for loading Application-level class path, path mentioned in environment variable, etc..
                            -->From java 9, we can call "Application Class Loader" as  "System ClassLoader".

                 -->Linking
                      -->verify -->Bytecode verifier will verify whether the generated bytecode is proper or not.
                      -->Prepare -->For all static variables memory will be allocated and assigned with default values.
                      -->Resolve -->All symbolic memory references are replaced with original references from Method Area.
                -->Initialization -->we assign original values to the static variables and static blocks get executed.
             2)Memory management or Run time Data Area:
                  -->Method Area
                       -->The "Method Area" is Loading Class Level Data.
                       -->All the static Data will be stored in 'Method Area".
                  -->Heap Area
                       -->The "Heap Area" is Loading Object Level Data.
                       -->All the Instance data Will be Stored in "Heap Area".
                  -->Stack Area
                        -->Executing the method When we Called is happening inside the Stack Area, When Main  method and all other methods after completing 
                            execution will be removed from Stack Area.
                  -->PC Registers -->They will hold the address of the current executing instruction once execution is completed they will updated with next 
                                      instruction.
                  -->Native Method Stack -->native method stack holds the native method area information.
              3)Execution Engine
                   -->Interpreter 
                         -->Converts byte Code into machine level language to execute.
                   -->JIT(Just-In-Time) Compiler : suppose if we call a method for many times in main method then the JVM will go to the interpreter only once 
                     and remaining time the JIT Compiler  will take care of it , that is the use of JIT(i.e. used for better performance of Java Applications 
                     during runtime). 
                   -->Garbage Collection:
                        -->Garbage Collector Removes Unreferenced Objects.
                        -->This garbage Collection can be done in two ways:
                            -->By Making the reference variable as "Nullify(t=NULL)", and assigning one reference variable to other(t1=t).When we use any one of 
                               the above method we need to call garbage Collector(System.gc()) then the Garbage Collector will Call the Finalize() method and it 
                               will remove garbage value or nullify value from the memory.
              4)Native Method Libraries  -- This a Collection of Native Libraries which are required for the Execution engine.
                                            
              4)Java Native Interface(JNI) -- JNI will be interacted with the Native method libraries and provide the Native libraries required for the 
                                              Execution Engine.
================================================================================================================================================================
APPLICATIONS OF JAVA:-
==========================
  -->java is used in "DESKTOP APPLICATIONS"
  -->"MOBILE APPLICATIONS"
  -->"ENTERPRISE APPLICATIONS"
  -->"WEB APPLICATIONS"
  -->"EMBEDDED SYSTEMS"
  -->"GAMING".
================================================================================================================================================================
FEATURES OR ADVANTAGES OF JAVA:-
===============================
1)Java is Simple -->why? 
   -->It's Syntax is Simple.
   -->In java, They removed Complicated Features like Pointers and Introduced References(Address of the object).
   -->In java, We have AGC(Auto Matic Garbage Collection).

2)Java is High-level --> why?
   -->High level Means English language or Human Understandable Language but "OS" does not understand English language,
     it Understands Only Low level Language. 
  -->Then What we need to do..? --> Convert high level to low level.
  -->For conversion we need to follow two steps:-
     1)Compilation(JDK) --> Source code ---> byte code (.class extension)
     2)Execution(JVM)   --> byte code --> machine level language -->(Low level Language) --> os -->output.

3)Java is Platform Independent -->why?
  --> platform means: OS + Processor
  --> Java is Platform Independent because, Compiled source code(byte code) can execute on any platform(Os) using Java Virtual Machine.
  --> We should not share source code with anyone, we only share the .class file (byte code).

4)Java is Robust -->why?
  -->Robust means "Strong".
  -->Java is Robust Due to:
       -->Strong Memory Management
       -->Exception Handling
       -->Multi threading

5)Java is Secure --> why?
  -->Java is Secure due to it's :
       -->byte code verifier
       -->Access modifiers
       -->Encapsulation
       -->Abstraction
       -->No Explicit Pointers

6)Java is Object oriented Programming -->why?
    -->Everything in java is Object.
    -->It is not Purely object oriented because it supports primitive data types like int, char, byte, etc...
================================================================================================================================================================
-->What is meant by "public static void main(String[] arms)"?
     -->In public static void main(String arms[])
              -->public means direct access to the JVM(Java virtual machine).
              -->static means direct access to the JVM(Java virtual machine)  but without creating any object.
              -->void means where as main function does not return anything.
              -->main means, it is callable environment to the java programs  where we can call user defined and pre-defined functions.
              -->why "String arms[]"(String array arguments)? :- if you want to send arguments through command line then we need to go for "String[] arms".
-->We can give "synchronized, strictfp, final" keywords for main method other than static..
-->CLA(Command Line arguments)
-->variable argument:-
       void m1(int ...a){
       }

-->sop(System. out. println):-
--------------------------------
-->"System" is a predefined class from Java. Lang Package.
-->"out" is a static variable in system class and referring print stream class.
-->"println" is a method from print Stream class.
-->We have total of 10 println methods with all primitive data types and object datatypes as arguments.
-->import static java.lang.System.out;
   out.println("Hello World");
================================================================================================================================================================
DIFFERENCE BETWEEN C++ AND JAVA:-
=======================================================
--> C++                                                                JAVA
   ======================                                       =====================================
    1.It is plat-form dependent                                    1.It is plat-from Independent
    2.It is mainly used for system programming                     2.It is mainly useful for application programming
    3.It supports go to statement                                   3.It doesn't supports go to statements
    4.It supports multiple inheritance                              4.It doesn't supports multiple inheritance through class. It is achieved through interfaces.
    5.It supports structures and unions                            5.java doesn't supports structures and unions.
    6.c++ supports pointers and we can write a pointer program     6.java does not supports pointers instead they developed references(address of the objects)
    7.c++ supports operator overloading                            7.java doesn't supports operator overloading.
================================================================================================================================================================
WHAT DOES A CLASS  CONTAIN:-
==============================
1) Data Members:
        -->Static Data members(variables + Methods)
        -->instance Data Members(Variables + Methods)
2)Blocks:
    -->Static Blocks
    -->Instance Blocks
3)Constructors:
      -->default
      -->Parametrized Constructor
4)Interfaces
5)Inner Classes
---------------------------------------------------------------------------------------------------------------------------------------------------------------
WHAT IS CLASS:-
==============
-->Class is a Blue Print(plan) of an object or it is a Template.
-->We can call class as a user defined data type.
-->By Default class extends from Object in java.
-->class is a static memory allocation.

WHAT IS OBJECT:-
==================
-->An Instance(Example) of a class is called an object.
-->Object is a Dynamic Memory Allocation.
-->Object is a real time entity.
-->Object consists of state , behavior and Identity.
Note: Where as Class is Dummy and Object is Real.
-->The Java Compiler will provide default constructor for your class to create an object.

creating object:-
-----------------
-->Class Name A = new Class Name();
          or
    new Class Name();
================================================================================================================================================================
READING INPUT IN JAVA:-
========================
Scanner class:- Scanner Class is a predefined class in "java. util" package
  -->Scanner sc=new Scanner(System.in); 
     byte r   =sc.nextByte();
     short m  =sc.nextShort();
     int n    =sc.nextInt();
     long s   =sc.nextLong();
     double w =sc.nextDouble();
     float f  =sc.nextFloat();
     String q =sc.nextLine(); or sc.next();
     Char ch  =sc.next().charAt(0 or i);
================================================================================================================================================================
-->To find Number of digits in the given number use this logic: (int)Math.log10(num)+1;
-->TO separate the digits from first then use the below logic:
        while(num>0)
        {
           int r= num/(int)Math. Pow(10,d) ;
           num=num%(int)Math. Pow(10,d);
        }
================================================================================================================================================================
PRINTING OUTPUT:-
==============================
* System.out.println("Java Fundamentals");
* System.out.println(x);
* System.out.println("Java :"+ x);
* System.out.print("Jaava Fundamentals");
* System.out.print(x);
* System.out.print("java:"+x);
* System.out.printf("%.2f" , x);
* System.out.format("%.2f", x);
================================================================================================================================================================
"JAVA LANGUAGE FUNDAMENTALS":-
=====================================
JAVA IDENTIFIERS:-
============================
-->java identifiers are used for identification purpose (or) Any name of the Project, package, class, interface, Method, variable is called as Identifier.
-->valid identifiers:-->($,_,[A-Z],[a-z],[0-9])-->but should not start with numbers.
-->Invalid identifiers:-->(@,#,%,-,...)

  RULES FOR IDENTIFIERS:-
------------------------------------------------------------------
   1)Java Identifiers can use (a-z) or (A-Z) or (0 - 9).
   2)Java Identifiers should not start with numeric values(0 -9)(Syntax error at token 1).
   3)Java Identifiers should not contain any Special Characters except "_" and  "$" , we can start identifiers with "_" or "$".
   4)Java Identifiers should not be a Java Keywords.
================================================================================================================================================================
JAVA KEYWORDS:-
==================
"Primitive Datatypes(8), Application level or oops(14), Access Modifiers(12), Exception handling(5), Logical Statement(11)"
PRIMITIVE DATATYPES KEYWORDS:-
-------------------------------
For Representing The Numbers:
  -->byte
  -->short
  -->int
  -->long
------------------------------------------
For Representing floating Decimals:
  ->float
  ->double
----------------------------------------------------------
For Representing characters and true or false conditions:
  ->char
  ->Boolean
----------------------------------------------------------------------------------------------------------------------------------------------------------------
APPLICATION LEVEL (OR) OOPS KEYWORDS:-
---------------------------------------
 -->"package" :- package is a keyword to create package for collection of classes and interfaces.
 -->"import"  :- To import classes or interfaces or Enums  from one package to another package.
---------------------------------------------------------------------------------------------------
 -->"class"    :- Class is a blue print of an object or template or user defined datatype.
 -->"interface":- interface is Blueprint of a class. 
 -->"Enum"     :- To represent constant values we use Enum like a class.
 -->"new"      :- new keyword is used to create object for a class.
 -->"instance of" --> to check status of the object from another object.
---------------------------------------------------------------------------------------------------
-->"void" -->return nothing
-->"return"  -->return something in a method based on the return type.
--------------------------------------------------------------------------------------------------
-->"this" :-> this Keyword is used "To invoke current object data members".
-->"super" :-> super keyword is used "To invoke super object data members".
-->"implements" 
-->"extends"
-->"assert"
---------------------------------------------------------------------------------------------------------------------------------------------------------------
ACCESS MODIFIERS KEYWORDS(12):-
--------------------------------
-->"private" :-  private is a keyword, we cannot  use for a class but we can use inside the class.(The Scope of private is within  the class).
-->"<default>" :- The Scope of default is within the package.
-->"protected" :- protected is a keyword , we cannot use for a class but we can use inside the class.(The Scope of Protected is "within the package + outside of the packages of subclasses:).
-->"public" :- public is a keyword we can user for a class and also we can use inside the class. (The Scope of public is within the project Anywhere).
---------------------------------------------------------------------------------------------------------------------------------------------------------------
-->"abstract" :- abstract is a keyword 
                      --> we can use for methods for declaration but not for implementation
                      --> we can use for classes for not creating an object to our class.
-->"static"   :-  static is a keyword we can use for data members and blocks. 
                  if we use static for a variable or data then it is constant for all objects.
                  if we use static for a method or blocks then it will loading to  the memory without creating object.
-->"strictfp" :-  strictly follows floating point data in all the systems.
-->"synchronized" :-synchronized is a keyword , we can go and use in multithreading to achieve synchronization.
---------------------------------------------------------------------------------------------------------------------------------------------------------------
-->"final" :-  final is for class then we cannot extends that class.
               final is for method then we cannot override that method in child class.
               final is for variable then we cannot change the value.
-->"transient":- transient is a keyword we can use it in serialization concept.
-->"Volatile" :- volatile means keep on changing , we can use it in multithreading when the threads are sleeping still you want to make your variables to change  the values.
-->"native"
---------------------------------------------------------------------------------------------------------------------------------------------------------------
EXCEPTION HANDLING(5):-
------------------------
-->try
-->catch
-->finally
-->throw , throws
----------------------------------------------------------------------------------------------------------------------------------------------------------------
LOGICAL STATEMENT:-
--------------------
-->if
-->else
-->for
-->while
-->do while
-->switch 
-->case
-->continue
-->go to
-->const
================================================================================================================================================================
JAVA  DATATYPES:-
=======================================
-->There are Two types of Data types in java : they are "Primitive Data types " and "Non-primitive datatypes"
-->Primitive datatype's in java are pre-defined by a java language and named as the reserved keywords. 
-->As primitive datatypes does not share a state with other primitive values. The Data in data types is stored in a 2's complement way. ( -2^n to 2^n-1)
-->byte (Byte)        ->size->1byte(8 bits)-->max value we can store in byte is 127 and min value is -128 -->byte bytevar;
                                                                                                (Byte.SIZE,Byte.MAX_VALUE,Byte.MIN_VALUE);
-->short(Short)       ->size->2bytes(16 bits)-->max value we can store in short is 32767 and min value is -32768 -->short shortvar; 
                                                                                                (Short.SIZE,Short.MAX_VALUE,Short.MIN_VALUE)
-->int(Integer)      ->size->4bytes(32 bits) -->max value we can store in int is 214748 and min value is -2147483647 -->int intvar; 
                                                                                                (Integer.SIZE,Integer.MAX_VALUE,Integer.MIN_VALUE)
-->long(Long)        ->size->8bytes(64-bits)-->long longvar;          
                                                                                                (Long.SIZE, Long.MAX_VALUE,LONG.MIN_VALUE)                                       
-->float(Float)      ->size->4bytes(32 bits)-->float floatvar;
                                                                                                (Float.size(), Float.MAX_VALUE,Float.MIN_VALUE)
-->double(Double)    ->size->8bytes(64 bits)-->double doublevar;
                                                                                                (Double.size(), Double.MAX_VALUE,Double.MIN_VALUE)
-->boolean           ->size->1bit  -->boolean boolvar;
-->char              ->size->16-bits-->char charvar; ( 0 to 65535) -->char data types is a single 16-bit Unicode characters.
-->All integers can be characters(by the concept of ASCII Values) and all Characters can be a integers.
----------------------------------------------------------------------------------------------------------------------------------------------------------------
Non-Primitive Data types(Wrapped object data types, pre-defined object data types, user-defined object data types):-
====================================================================================================================
-->String        
-->StringBuffer   
-->Math
-->BigInteger 
      -->It is a predefined class and predefined object datatype , it can store value larger than "int" and "long".
      -->synatx:-  BigInteger b= new BigInteger("232097329209027598383833793830383");
                   BigInteger b1= new BigInteger("2320973292090275983834865484646438463830383");
      -->Following are some the methods that BigInteger have:
              -->b. add(b1);
              -->b. multiply(b1);
-->BigDecimal
       -->BigDecimal b2=new BigDecimal("467686969670707.6868686868");
-->Student, Employee, Address,....(user-defined object datatypes)
-->"NULL" is the Default value of any object data type.
================================================================================================================================================================
JAVA TYPECASTING:-
====================
Type Casting:-
---------------
Type Casting is nothing but, conversion of one data type to another data type.

There are two types of type casting they are:-
  
1)Widening or implicit or Automatic Type Casting:-
--------------------------------------------------
  Converts smaller data type to larger data type.

  byte-->short-->char-->int-->long-->float-->Double

 example:-
    long x=12345567;
    float f=x; //implicit type casting

2)Narrowing or explicit or Manual Type casting:-
------------------------------------------------
  converts larger data type to smaller data type.
  
  double-->float --> long-->int-->char-->short-->byte
 
  Example:-
  
     double y=123456.78;
     int z=(int)y; //Explicit Type casting

-->All primtive data types can be converted to wrapper Object data Types, and that process is known as Auto Boxing
  
  int x=99;
  Integer y=x;

-->All Wrapper Object data types can be converted to Primitive data types, and that process is known as Auto UnBoxing.

   Integer y=99;
   int x=y;

-->All Strings can be converted to Wrapper Object data types by using following methods:
  
    String s="123.897";
   
    int res=Double.parseDouble(s);
===============================================================================================================================================================
JAVA WRAPPER CLASSES:-
=======================
-->Java Wrapper classes provides a way to use primitive datatype's as objects.
--->  Primitive datatypes                Wrapper Object Data Types
     ========================          ==============================
       byte(8bits)              -->      Byte
       short(16 bits)           -->      Short
       int(32 bits)             -->      Integer
       long(64 bits)            -->      Long
       float(16 bits)           -->      Float
       double(32 bits)          -->      Double
       char                     -->      Character
       boolean(1 bit)           -->      Boolean

-->For converting one primitive datatype to another datatype we have type casting but to one type to another type by using wrapper class objects we have :
     -->byteValue();
     -->shortValue();
     -->intValue();
     -->longValue();
     -->floatValue();
     -->doubleValue();
     -->charValue();
     -->toString();
-->example:-
  ==========
  import java. util.*;
    public class M{
        public static void main(String args[]){
                Integer a = 5;
                Float f = 5.66;
                Character c = 'A';
           System.out.println(a);
           System.out.println(f);
           System.out.println(c);
           System.out.println(f.intValue());
           System.out.println(a.doubleValue());
          System.out.println(c.toString());
       }
   }
===============================================================================================================================================================
JAVA LITERALS:-
=================
-->Literal is a Constant value which we are storing it into a variables.
-->Java Language Specifies Five Major types of literals, they are:
       --Integral Literals
             --Decimal Literals (Decimal Numbers starts  as a normal number and its range is 0 to 9)
             --octa Decimal Literals(Octa Decimal Numbers prefixed with "0")(range 0 to 8)
             --Hexa Decimal Literals(Hexa Decimal Numbers prefixed with "0X" or "0x") (range 0 to 9, a to f)
       --Floating Literals -->octa and hex decimal literals are not possible for double datatype.
       --char Literals -->char data types is a single 16-bit Unicode characters.
       --Boolean Literals -->(true or false)
       --null literals -->most of the object reference variables are assigned with null value.
       --String Literals
-->Literals can be any Number  or text or other information that represents a value.
-->We will use Literals in addition to variables in java  statements.
================================================================================================================================================================
TYPES OF VARIABLES:-
=====================
-->DIVISION 1:-
--------------
   -->Based on type of value represented by a variable all variables are divide into two types:
          "Primitive variables" : can be used to represent primitive values.
          "object variables"    : can be used to refer to objects.
---------------------------------------------------------------------------------------------------
-->DIVISION 2:-
---------------
   -->Based on behavior and position of declaration all variable are divided into three types :
        1) "Instance variables" :
             -->The value of Instance variables varies from object to object.
             -->For every object a separate copy of Instance variable will be created.
             -->Instance variable will be created at the time of object creation and destroyed at the time of object destruction.
             -->Instance variables will be loaded in to the Heap Area when object is created.
        2) "Static Variables" :
              -->The Value of Static variables will be remain constant for all objects.
              -->For Any object , only one copy of static variable will be created.
              -->Static variables will be created at class level and loaded in to the method Area.
        3) "Local Variables" :
              -->The Local variables will be created inside the main method.
              -->Duplicates can be allowed to this variables.
              -->JVM is Not responsible for loading these local variables.
-->Compared to static , instance and local , the highest priority will be given to local variables.
================================================================================================================================================================
TYPES OF METHODS:-
====================
why we need Method?
--------------------
The main aim of creating methods is to reuse the code any number of times in anywhere in the project.

what is..method?
----------------
-->Method means it's a behavior of a class.
                or
-->Method means Collection of logics and collection of statements.
                or
-->Method is a block of code which execute when we called.
-->We cannot write one method inside another method.
-->we can write a block inside of the Any Method.
-->we can call one method in another different method.
-->we can call the method in same method but we will get stack overflow error.

-->There are 4 types of methods they are:
    -->Method with no "return type" and with "no arguments".
    -->method with "return type" and with "no arguments".
    -->method with "no return type" and with "arguments".
    -->method with "return type" and with "arguments".
Example Program:-
====================
package com. sample;
import java. util. Scanner;
public class TypesofMethods4 {
     static Scanner sc = new Scanner(System.in);
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		TypesofMethods4 t = new TypesofMethods4();
		t.m();
		t.m1(10,20);
		int age = t.m2();
		int sum= t.m3(2333, 333);
       //t.m3(int x=2, int y=3) --->We cannot pass arguments in this way -->it will give token error.
		System.out.println("my Age is:"+age);
		System.out.println("my sum is:"+age);
        
	}
	
	void m()   //With "No return Type" and with "No arguments"
	{
		System.out.println("Hai Ajay");
	}
	 
	void m1(int x , float y) {    //method with "no return type" and "with arguments"
		System.out.println("Sum of two Numbers is:"+(x+y));
		
	}
	
	int m2() //method "with return type" and "with no arguments"
	{
		System.out.println("enter your age:");
	  int age = sc.nextInt();
	  return age;
	}
	
	int m3(int x, int y) //method "with return type" and "with arguments"
	{
		return (x+y);
	}

}
================================================================================================================================================================
JAVA CONSTRUCTORS:-
=====================
Why We need Constructors..?
----------------------------------------------------------------------------------------------------------------------------------------------------------------
     -->To Initializing an object and initializing instance data but not static data  we need Constructor.
     -->Without Constructor there is no chance to create the object.
----------------------------------------------------------------------------------------------------------------------------------------------------------------
What is Constructor..?
----------------------------------------------------------------------------------------------------------------------------------------------------------------
-->Constructor is a special member function which is used to initialize an object. When Object is created constructor get invoked Automatically.
----------------------------------------------------------------------------------------------------------------------------------------------------------------
What are the Types of Constructors:-
-----------------------------------
1)Default constructor:-
 -------------------------
  why-->If our class does not contain any type of constructor(no-args, parameterized) then the java compiler is providing a constructor and that constructor is called as 
  default constructor.

2)Parameterized constructor:-
 ----------------------------
 why-->While creating an Object if we want to send any values to that Object then we will go for the concept of Paramtereized Constructor.
 
 The constructor which takes the arguments as a Input,that constructor is called as Parameterized Constructor.

3)No args Constructor:-
---------------------------
  why-->If our class contains parametrized constructor but if we want to create an Object without values then we will go for the concept of No args Contructor.
 
  The Constructor which does not take any arguments as inputs,that constructor is called as No args Constructor.

-->"this" is a keyowrd to invoke current class Object data members.
-->"super" is a keyword to invoke super class Object Data members.
-->"this()" is a method to call current class constructor.(Single Class)
-->"super()" is a method to call super class Constructor.(Multiple Classes)

4)Constructor chaining:-
 -----------------------
  If we are calling one constructor inside Another constructor by using "this()" (In case Single class) and "super()"(In case of Mutltiple classes) methods is called as 
  constructor chaining.

5)Copy constructor:-
 ---------------------
  If we are copying one constructor in to another constructor by using Object reference variable is called as Copy constructor.
----------------------------------------------------------------------------------------------------------------------------------------------------------------
RULES FOR CONSTRUCTORS:-
----------------------------
1) The class name and constructor name should be same.
2) constructors should not return anything even void.
3) Applicable Access Modifiers for the constructors are below:-
      -->private
      -->protected
      -->default
      -->public
Note:other than the above modifiers if we give any other modifiers then we will get the compile time error.
4) "this()" and "super()" methods must  be in the first line of any constructor.
5) "this()" and "super()" methods must need to be call inside the constructor only but not in methods.
6) If our class does not contain any constructors then the java compiler is providing a constructor and that constructor is called as default
  constructor.
7) If our class contains any of the constructor then the java compiler is not going to provide any default constructor.
8) If our class contains parameterized constructor but if we want to create an Object without values then we will go for No args constructor.
9) "this" and "super" keywords are used to invoke current class and super class Object data members and both can be used in constructors and methods but not in 
    static methods.
10) Constructors can be overloaded.
11) Both "this()" and "super()" methods cannot be used at a time in a constructor.
12) The scope of default constructor is scope of the class.
================================================================================================================================================================
JAVA ARRAYS:-
=================
Why wee need Arrays?
----------------------
       -->structuring the data in a proper way from unstructured data.
       -->It is More Readable to maintain the code.
       -->To maintain continuous memory allocation.

What is Array?
--------------
 -->Array is an object.
 -->Array is a index based, collection of homogeneous data elements into a single unit with fixed size.
 -->Array is a fixed and mutable(i.e. we can replace the value of a array element)

Array Creation:-(For Creating an array we need to follow four steps they are: Declaration, Creation, Initialization, Representation)
=================
1) Declaration
    --> int[] ages;
2)Creation
    ages = new int[n]; //n is the size and index is "0 to n-1"
   Note: while creating an array, we must specify the size.
3)Initialization
    ages[0] = 22;
    ages[1] = 23;
    ages[2] = 24;
    ages[3] = 25;
4)Representation.
    //for(Initialization; condition; increment/decrement){}
    //Initialization : where you want to starts from : int i= 0
    //condition     : up to where u want to go ?: i<100
    //Increment     :  Initial values incremented by +1: i++
   for(int i=0;i<n; i++){
     System.out.println(ages[i]);
   }

-->The Maximum Range of Array is : Integer maximum value(2147483647).
-->We can create and initialize an array in a single line by using "{}".

//Reading the elements from console using scanner class..
---> for(int i=0;i<size; i++){
       A[i] = sc.nextInt();
   }
//for-each loop or enhanced for loop
-->for(int i : A){
    System.out.println(i);
   }

2D Arrays:-
==============
Whenever you want to represent rows and columns we need to go for 2Dimensional arrays.
syntax:-
-->int[][] A = new int[3][3];
          (or)
-->int[] A[] = new int[3][3];
for(int i=0;i<A. length; i++){
  for(int j=0;j<A[i].length; j++){
     System.out.println(A[i][j]);
  }
}
-->for(int[] n1 : A){ //for -each loop for 2D array.-->first convert 2D to 1D array and then 1D to normal Number.
      for(int n : n1){
         System.out.print(n+" ");
      }
  }


JAGGED ARRAY:-
===============
-->Array of Arrays is called as jagged array.
 syntax:-
  int[][] A = new int[2][];
   A[0] = new int[4];
   A[1] = new int[3];

Example program for prime Number:-
======================================
import java.util.Scanner;
public class M{
   public static void main(String args[]){
       scanner sc =new  Scanner(System.in);
       System.out.println("Enter the size:");
       int s = sc.nextInt();
       int[] A = new int[s];
       System.out.println("Plz enter the array elements:");
       for(int i=0;i<s;i++)
       {
             A[i]=sc.nextInt();
        }
        System.out.println("Prime Numbers for the Array are:");
        for(int i=0;i<s;i++){
          boolean flag = true;
          for(int j=2;j<A[i];j++){
                if(A[i]%j==0){
                    flag = false;
                    break;
                }
           }
           if(flag){
              System.out.println(A[i]);
           }
         }
   }
}

Bubble Sort Algorithm:-
=========================
Bubble Sort Algorithm is the Simplest Sorting Algorithm that  works by repeatedly Swapping the adjacent elements if they they are in wrong order.
Time Complexity: o(n^2) -->Worst time complexity
Space complexity : o(1)

Example program:-
======================
class Main{
  public static void main(String args[]){
       int[] A = {39,19,15,12,5,6};
       int tmp=0;
       for(int i=0;i<A.length;i++){
        int flag =0;
         for(int j=0;j<A.length-1-i;j++){
             if(A[j] > A[j+1]){
                tmp=A[j];
                A[j]=A[j+1];
                A[j+1]=tmp;
                flag = 1;
         }
       if(flag==0){
          break;
        }
      }
     for(int c :A){
          System.out.println(c);
     }

Selection Sort Algorithm:-
===========================
Selection sort is a Straightforward sorting Algorithm that operates by repeatedly finding the minimum element
, from an unsorted section of array and moving it to the beginning. This process continues until the entire array is sorted.
Time Complexity : o(n^2)
Space Complexity: o(1)

Example Program:-
==================
public class Array{
    public static void main(String args[]){
       int[] A = {39,19,29,12,15,5};
       for(int i=0;i<A.length;i++){
           int tmp=0;
           int min=i;
           for(int j=i+1;j<A.length;j++){
                 if(A[j] < A[min]){
                       min = j;
                 }
           }
           tmp=A[i];
           A[i]=A[min];
           A[min] = tmp;
       }
       for(int c : A){
         System.out.print(c+ " " );
      }  

3Dimensional Array:-
====================
Declaration and creation:-
---------------------------
int[][][] A = new int[3][3][3];
       	 (or)
int[] A[][] = new int[3][3][3];
         (or)
int[][] A[] = new int[2][2][2];

initialization:-
----------------
A[0][0][0] = 111;
A[0][0][1]=  222;
A[0][0][2]=  333;

A[0][1][0] =444;
A[0][1][1] =555;
A[0][1][2] =666;

A[0][2][0]=777;
A[0][2][1]=888;
A[0][2][2]=999;

  (or)
int[][][] A = { { { 111, 0, 0 } }, { { 0, 222, 0 } }, { { 0, 0, 333 } }, { { 444, 0, 0 } }, { { 0, 555, 0 } },
				{ { 0, 0, 666 } }, { { 777, 0, 0 } }, { { 0, 888, 0 } }, { { 0, 0, 999 } } };

Representation:-
---------------
for(int i=0;i<A.length;i++){
   for(int j=0;j<A[i].length;j++){
     for(int k=0;k<A[i][j].length;k++){
        System.out.print(A[i][j][k] + " ");
     }
     System.out.println();
  }
  System.out.println();
}

//using for each loop:-
------------------------
for(int[][] n2:A){
  for(int[] n1:n2){
      for(int n : n1){
          System.out.print(n+" ");
      }
     System.out.println();
   }
System.out.println();
}
================================================================================================================================================================
ARRAYS CLASS:-
==================
  -->Arrays class is a built-in class in java that provides variuos utility methods for working with Arrays.
   Methods:-
        import java.uitl.Arrays;
        int[] Array={1,4,2,5,3,6,9};
       1) Arrays.sort(Array_name);   //sort the elements of the array in ascending order.
       2)int[] index=Arrays.binarySearch(Array_name,value); //search for specific element inthe array using binary search algorithm.
       3)boolean[] equal = Arrays.equals(Array1,Array2); //compares to Arrays for eqaulity.
       4)var list=Arrays.asList(Array_name);  //converts given array into the list.
       5)int[] copy=Arrays.copyOfRange(Array_name,value1,value2); //copies the specified range of Array elements to another Array.
       6)Arrays.fill(Array_name,value); //Fills specific value in to the array.
       7)Arrays.toString(Array_name)
================================================================================================================================================================
JAVA LOGICAL STATEMENTS AND OPERATORS:-
=========================================
1)simple "if" and "else":-(Decision Making)
---------------------------------------------
syntax:-
  if(condition){//true
       //block of statements
  }//if we are not taking curly braces to the if block then it is going to take only one statement.
 else{//false
    //block of statements
 }

2)"Nested if":-(Decision Making)
-------------------------------
syntax:-
 if(condition1){
     //block of statements
     if(condition2){
        //block of statements
        if(condition3){
           //block of statements
        }
     }
}

3)"Nested if-else":-(Decision making)
-------------------------------------
if(condition1){
   //block of statements
   if(condition2){
      //block of statements
  }
  else{
     //block of statements
 }
}
else{
   if(condition 3){
        //block of statements
  }
  else{
   //block of statements
  }
}

4)"if-else-if":-(Decision making)
--------------------------------
syntax:-
if(condition1){
    //block of statements
}
else if(condition2){
   //block of statements
}
else if(condition3){
  //block of statements
}

5) "switch statement":-(Decision making)
----------------------------------------
A switch statement in java is used to execute a single statement when there are multiple conditions.
syntax:-
char Ch;
switch(expression or Ch){
     case 1 : //block of code
              break;
     case 2: { //we can give curly braces
             //block of code
             break;
             }
       |   
       |
     case n: //block of code
             break;
     default: //block of code
             break;
} 
     (OR)
switch(expression){
 case 1 --> //block of statements;
 case 2 --> //block of statements;
   |
   |
   |
 case n --> //block of statements;
 default --> //block of code;

6) "WHILE LOOP":-(looping Statements)
  ------------------------------------
  -->It is also called as entry controlled loop.
 syntax:-
  initialization;
  while(condition-->Boolean){
      //block of code;
     increment/decrement; //breaking value
  }
 
7)"DO WHILE LOOP":-(looping statements)
---------------------------------------
-->It is also called as exit controlled loop.
syntax:-
initialization;
do{
  //block of code;
}while(condition);
----------------------------------------------------------------------------------------------------------------------------------------------------------------
OPERATORS:-
===========================================================
-->unary  operators:-(++(pre, post),--(pre, post))
   Post Increment: value will print first and then increment next.
   post Decrement: value will print first and then decrement next.
   pre  Increment: value will increment first and then print next.
   pre Decrement : value will decrement first and then print next.
-->Arithmetic Operators && shift operators:- (+,-,*,%,/, >>(right shift) or >>>,<<(left shift))
     -->Right shifting(>>) is nothing but division by 2 and Left shift(<<) is nothing but multiplication by2.
-->Relational operators:- (>,<,>=,<=,==,!=)
-->Logical operators:- (&&,||,!)
-->Assignment operators:- (variable=value, = ,+=,-=,/=,*=,%=,&=,|=,^=,<<=,>>=)
-->Ternary operator:- ((condition)?  true: false)
-->Bitwise operators:- (&,|,^)
-->instance of

Operators Precedence and Associativity(BODMAS):-
 ================================================
 1. unary operators have high precedence(+,-,++,--)
 2. ( ) -->parenthesis are having Second highest priority.(BO)
 3. *,/,% -->are having third highest priority.(DM)
 4. +(Addition) , -(Subtraction) -->are having fourth highest priority.(AS)
If we have same precedence operators in the equation:
  then for(*,/, %) the Associativity will be Left to Right.
  then for(+,-) the Associativity will be from Right to Left.
================================================================================================================================================================
JAVA ACCESS MODIFIERS/SPECIFIERS:-
====================================
-->"private"   :- private is a keyword, we cannot  use for a class but we can use inside the class.(The Scope of private is within  the class).
                 USED FOR--> (inner class, variables, methods, constructors)
-->"<default>" or undefined :- The Scope of default is within the package.
                 USED FOR--> (class, inner classes, variables, methods, constructors, interfaces)
-->"protected" :- protected is a keyword , we cannot use for a class but we can use inside the class.(The Scope of Protected is "within the package + outside of 
                  the packages of subclasses by using sub class object reference variables).
                  USED FOR -->(inner classes, variables, methods, constructors)
-->"public"    :- public is a keyword we can user for a class and also we can use inside the class. (The Scope of public is anywhere in the project).
                  USED FOR -->(class, inner classes, variables, methods, constructors, interfaces)
-->"final"     :- final is for class then we cannot extend that class.(inheritance is not possible)
                  final is for method then we cannot override that method in child class.
                  final is for variable then we cannot change the value of that variable.
                  USED FOR -->(class, inner classes, variables, methods)
-->"static"    :- static is a keyword we can use for data members and blocks. 
                  if we use static for a variable or data then it is constant for all objects.
                  if we use static for a method or block then it be will loading in to the Method Area without creating object.
                  static data remains constant for every object but instance data varies for object to object.
                  USED FOR -->(variables, methods, blocks)
-->"abstract"  :- abstract is a keyword 
                      --> we can use for methods for declaration but not for implementation
                      --> we can use for classes for not creating an object to our class.
                  USED FOR -->(class, methods)
-->"strictfp"  :-  strictfp is a keyword , which strictly follows floating point data in all the systems.
                  USED FOR --> (Class, methods)
-->"synchronized" :- synchronized is a keyword , we can go and use in multithreading to achieve synchronization.
                  USED FOR--> (Blocks, methods)
-->"transient"  :- transient is a keyword we can use it in serialization concept.(used for variables)
-->"volatile"(used for variables)
-->"native"(used for methods)
===============================================================================================================================================================
JAVA STRING HANDLING:-
======================
-->String is a Non-primitive datatype or object datatype.
-->String is a class from java.lang package.
-->String is Immutable(we cannot change the value of these  objects) object where as String Buffer and String Builder are Mutable(we can change the value of 
   these object) objects.
-->A Collection of characters which are represented into a single variable using "Double Quotes" is called a String.
-->String is a thread Safe.

--> There are 4 ways to create String:-
    1) String Literal:-
    --------------------
       String s = "Ajay"  -->Loaded into String Constant pool(SCP) --> Special memory from Heap area.

    2) String Object:-
    ----------------------
       String s1 = new String("Ajay1") -->Loaded into Heap Area.

    3) String Buffer:-
    -----------------------
      StringBuffer sb = new StringBuffer("ajay");

    4) StringBuilder:-
   --------------------------
     StringBuilder SB = new StringBuilder("ajay");


JAVA STRING METHODS:-
======================
1) "charAt(int index)" :- Returns the character at the specified index.(o/p:- character)
   eg:- char c = s.charAt(i);

2) "length()" :- Returns the Length of the String.(o/p:- integer)
    eg:- s.length();

3) "codePointAt(int index)":- Returns the unioce character at the specified index.(o/p:- return ASCII Value -->integer)
    eg:- int res = s.codePointAt(index);

4) "codePointBefore(int index)" :- Returns the unicode character before the specified index.(o/p:- integer)
    eg:- int res1= s.codePointBefore(index);

5) "equals(String s1)" :- Compare  String "s" with another String "s1".(o/p :- returns true or false)
    eg:- boolean  res= s.equals(s1);

6) "equalsIgnoreCase(String s1)" :- Compare String "s' with another String "s1" ignoring case considerations.(o/p:- return true or false)
    eg:- boolean res1= s.equalsIgnoreCase(s1);

7) "compareTo(String s1)" :- Compare two Strings lexicographically(based on ascii values).(o/p:- integer)
    eg:- int res= s.compareTo(s1);

8) "compareToIgnoreCase(String s1)" :- Compare two Strings lexicographically, ignoring case differences.(o/p:- integer)
    eg:- int res1=s.compareToIgnoreCase(s1);

9) "concat(String s1)" :- concatenate String "s1" to the end of String "s".(o/p:- String)
   eg:- s=s.concat(s1);

10) "contains(character sequence c)" :- Returns true if and only if the character 'c'  present in the character sequence of a String "s".(o/p:- boolean)
    eg:- boolean res = s.contains("a");

11) "toUpperCase()" :- Converts all the characters of a String "s" in to Upper case.(o/p:- String)
   eg:- s.toUpperCase();

12) "toLowerCase()" :- Converts all the characters of a String "s" in to Lower Case.(o/p:- String)
    eg:- s.toLowerCase();

13) "trim()" :-  To remove leading and trailing spaces in a String "s" we need to go for "trim()" method.(o/p:- String)
    eg:- s.trim(); -->System.out.println(s.trim());

14) "replace(charSequence target or delimter , charSequnce replacement)" :- To remove spaces in between a String based on Strings.(o/p:- String)
     eg:- s.replace(" ", "");

15) "replaceAll(String regexp, String replacement)" :- To Remove spaces in between a String based on regular expressions.(o/p:- String)
    eg:- s.replaceAll(" ", "@");

16) "replaceFirst(String regexp, String replacement)" :- To Remove First space in between a String based on regular expressions.(o/p:- String)
    eg:- s.replaceFirst(" ", "@");

17) "split(String regexp)" :- Splits this string around matches of the given regular expression.(o/p:- array of String)
    eg:- String[] S2 = s.split(","); or String[] s2= s.split("//s");

18) "split(String regexp, int limit)" :- Splits this string around matches of the given regular expression.(o/p:- array of Strings)
     eg:- String[] s2= s.split("," , 3);

19) "indexOf(int ch)" :- Returns the index of first occurence of a given subString within this String "s".(op:- integer)
    "indexOf(int ch, int fromIndex);
     eg:- s.indexOf('a');

20) "lastIndexOf(int ch)" :- Returns the last index of a given subString within this String "s".(o/p:- integer)
     eg:- s.lastIndexOf('a'); 

21) "isEmpty()" :- Returns true if and only if the length() is "0".(o/p:- boolean)
     eg:- boolean res= s.isEmpty();

22) "toCharArray()" :- converts the given String into Array of Characters.(o/p:- char Array)
     eg:- char[] ch = s.toCharArray();

23) "substring(int beginindex)" :- Returns the String that is a subString of this String.(o/p:- String)
      eg:- s.substring(5); 

24) "substring(int beginIndex, int lastIndex)" :- Returns the String that is a subString of this String.(o/p:- String)
     eg:- s.substring(3,7);

25) "valueOf(int , byte,short, long,float,..)" :- Returns the String representation of  all the  primitive arguments.
     eg:- int a1=100;
          String a2=String.valueOf(a1);
26) "toString()" 

27) "Character.isDigit(ch);" :- It will return true or false based on it is digit or not.
  
28) "Character.getNumericValue(ch);" 
     
29) "Character.isUpperCase();"
     
30) "Character.isLowerCase();"
     
31) "Character.toUpperCase(ch);"
    
32) "Character.toLowerCase(ch);"

33) "intern()" :- Returns the canonical representation of a given String.(strng)
     eg:- s.intern();  s1.intern();
===============================================================================================================================================================
STRING BUFFER && STRING BUILDER IN JAVA:-
============================================
StringBuffer:-
-------------
-->StringBuffer is a mutable Object(we can chage the value of these objects).
-->StringBuufer is a thread safe.
-->StingBuffer is a synchronized because its methods are thread safe and can be used in multithreading environment.
-->The Default Capacity of StringBuffer is 16.

StringBuilder:-
----------------
-->StringBuilder is also a mutable Object(We can the value of these objects).
-->StringBuilder is not a thread Safe.
-->StringBuilder is not synchronized, because its methods are not thread safe and cannot be used in multithreading environment.
-->The Default capacity of StringBuilder is also 16.

                        String                        StringBuilder                       StringBuffer
                      ------------                  -------------------                 ----------------------
Mutability->           Immutable                        Mutable                              Mutable

Thread Safety->        Thread Safe                    Not thread safe                       Thread Safe

Memory Efficiency->    High (SCP)                    Efficient(heap area)                   Less Efficient(heap Area)

Performance->          High(No-synchronization)       High(No-synchronization)              Low(due to synchronization)

usage->               This is used when we            This is used when thread              This is Used when thread safety 
                      Want immutability                Safety is not required.              is required.


syntax:-
--------
 StringBuffer sb = new StringBuffer();

StringBuilder:-
--------------
-->StringBuilder is a mutable object.
================================================================================================================================================================
JAVA OOPS:-
============
-->OOPS stands for object oriented programming structure or system.

WHY...?
-----------
--> To write a Program in a structured or organized or proper way, we must need to  go for oops.

WHAT... is OOPS?
----------------
--> If any program consists of below principles then we can call it  as object oriented programming.
      1)Encapsulation -- Security or Modularity (use)
      2)Abstraction   -- Security or flexibility (use)
      3)Inheritance   -- Reusability(use)
      4)polymorphism  -- Flexibility(use)

where... we use?
-----------------
--> Without OOPS , we cannot even write any simple java program, even it is very simple java program we are using oops.    
----------------------------------------------------------------------------------------------------------------------------------------------------------------

ENCAPSULATION:-
=======================
-->It is a Combination of :
        - Data Hiding --> Hiding the data
             +
        - Abstraction --> Hiding the implementation.

-->Encapsulation means, Binding the data or Wrapping the data or bundling the data with "related functionalities" in to a single unit.
-->JAVA API is the best example of Encapsulation Mechanism.
-->In MySQL , Normalization is the best example of Encapsulation.
-->Each and every class in java is following encapsulated mechanism.
-->The Object in Encapsulated class is called as DTO(Data transfer object) or PLOJO(Plain old java object) or Data Model

Data Hiding(To work on Encapsulation) :- This can be achieved by the following three terminologies:
      - we need to stop the access.                --> private keyword
      - we should provide the modification option. --> setters method
      - we should provide the readability option.   --> getters method

why Encapsulation..?
--------------------
-->To Achieve Security or Modularity.
-->"let us say , we are having a database that consists of data , and how this data is transferring to the UI, means, we are having a object in java class with same name as table name and the fields of database are my java class variables, Now i need to secure my data from others accessing directly and i will provide 
only modification by  using setter method and readability by using getters method."
----------------------------------------------------------------------------------------------------------------------------------------------------------------

Abstraction:- 
==============
-->Abstraction is the process of "Hiding the Implementation" and "showing only essential information" to the users.
-->By Using "Interface" and "abstract" keywords  we can achieve Abstraction.
-->ATM machine is one of the best example of Abstraction.

Interface:-
------------
-->Interface is a keyword used to create interface types.
-->Interface is a blue print of class.
-->Interface is a SRS(service Requirement Specification) but not implementation.
-->Interface is a contract between client and developers.
-->For Interface we cannot create an object.
-->Interface can extends any number of interfaces where multiple inheritance is possible with interface.
-->If we want to Implement "interface methods" we must need to use "implements" keyword in classes.
-->In Interface there are no constructors.

why interface..?
--------------------
-->if we want 100% abstraction then we will go for interface concept.

There are three types of Interfaces:
--------------------------------------
1) Normal Interface:-
      --> up to 1.7 version:- A interface can contain "any number of abstract methods" + " static variables".
      --> From 1.8 version:- In Interface we can have "default methods" and "static methods".
                           why?   -->"default methods" will help "to achieve the Backward Compatibility".
                                  -->"default methods" can be override.
                           why?   -->"static methods" will help "to provide constant behavior for all implemented classes"
                                  -->"static methods" cannot be override.(this is the difference between default and static).
                                  -->we cannot call static methods by using "reference variables" , we can call them by using "interface names".
      --> From 1.9 version:- In Interface we  can have "private methods".
                            why? -->"Private Methods" will help to remove duplication from default methods.
    example:- Collection, List, Map, Set.

2) Functional interface:-
      -->An Interface which contains only one "Abstract Method" is called as Functional Interface.
   example:- Comparable, comparator.

3) Marker Interface:-
     -->An Interface which does not contain any methods is called as marker Interface.
  example:- cloneable, serialization, Random Access.


Abstract Class:-
----------------
-->Abstract is a keyword:
     -- we can use for methods for declaration but not for implementation.
     -- we can use for classes for not creating an object of that class. 

why we need "abstract class"...?
--------------------------------
-->Whenever we don't want to create an object for our class then we need to go for "abstract class".
-->if we need "100%" abstraction we need to go for "interface" but if we need "0 to 100 %"(10 or 20%) abstraction we need to go for "abstract class".

              abstract class                                               interface
         ---------------------------                              -----------------------------
1)  Abstract class can have abstract and                         1)Interface can have only abstract methods, since java8 it can have default
    non-abstract methods.(regular, concrete)                         methods and static methods.
2)  Abstract class can have constructors.                        2)In Interface there no constructors.
3)  Abstract class does not support multiple inheritance.        3)Interface supports multiple inheritance.
4)  Abstract can have final, non-final, static and               4)Interface can only have static and final variables.
    non-static variables.
5) The "abstract" keyword is used to declare                     5)The "Interface" keyword is used to declare Interface.
   abstract class.
6) Data Members of a java abstract class are private,            6)Data Members of a java interface are public by default.
   protected...

example:-
----------
Interface In1
10 abstract methods 

abstract class AB1 implements In1{
  //We are implementing all the 10 abstract methods in abstract class without functionalities and creating like dummy implementation.
  //These Methods are called as concrete methods.
}
class A1 extends AB1{
  2 methods
}
class A2 extends AB1
{
  3 methods
}
class A3 extends AB1{
  4 methods
}

Note:-
--------
In Abstract class, we can have abstract methods, concrete methods, static and instance variables, regular methods, constructors.
If a class is "abstract" then we no need to have "abstract methods" but if our class contains "abstract methods" then that class must be a "abstract class".

Benefits of Abstraction:-
--------------------------
-->Security
-->flexibility
================================================================================================================================================================
INHERITANCE:-
===================
why inheritance..?
----------------------
-->Whenever we are looking for "Reusability" then we will go for inheritance.

what is inheritance..?
-------------------------
-->Inheritance means "IS-A Relationship" and also we will consider as "HAS-A Relationship".
-->Getting Data members or properties from parent class to child class is the concept of Inheritance.

Where we use inheritance..?
------------------------------
-->Everywhere in java , without inheritance there is no single java program.

-->"extends" is the keyword used to achieve inheritance.
-->By using child class reference and child class object we can call both child class and parent class functionalities.
-->By using parent class reference and parent class object we can call only parent class functionalities but not child class.
-->By using parent class reference and child class object we can call only parent class functionalities but not child class directly, where we 
   can call child class methods which are override.(upcasting)
-->Storing parent object and child reference is not possible in java because parent class is not extended by the child class.
 (Down casting is not possible in java directly but with explicit type casting we can call both child and parent class functionalities)

Types of Inheritance:-
-----------------------
-->implicit inheritance
-->single level inheritance
-->multi level inheritance
-->multiple inheritance -->it is not possible in java for classes but it will be possible for interfaces.
-->Hierarchical inheritance
-->Hybrid inheritance
-->cyclic inheritance-->It is not possible in java.

1)Single Level Inheritance:-
----------------------------
               A(super class)
               |
               B(sub class)
example:-
class A{
}
class B extends A{
}

2)Multi Level Inheritance:-
-----------------------------
            A(super)
            |
            B(intermediate class)
            |
            c(sub)
example:-
class A{
}
class B extends A{
}
class c extends B{
}

3)Multiple Inheritance :-
-----------------------
Multiple Inheritance is not possible in java for classes. It is possible for interfaces.
Example:-
class A{
}
class B{
}
class c extends B,A{
}

4)Hierarchical Inheritance:-
-----------------------------
      A(super)
      |
    -----
    |    |
    B    C -->sub classes

example:-
class A{
}
class B extends A{
}
class C extends A{
}

5)Hybrid Inheritance:-
-----------------------
-->It is a combination of two or more types of inheritance.
example:-

 interface A{
 }
 class B{
 }
 class C  implements A extends B{
 }

6)cyclic Inheritance:- It is not possible in java.

Benefits(why):-
---------------
-->Code Reusability
-->Readability
-->Memory efficiency
================================================================================================================================================================
POLYMORPHISM:-
==================
Why we need to go for polymorphism..?
--------------------------------------
    --Flexibility, readability or loosely coupling.

what is polymorphism:-
------------------------
-->polymorphism means "many forms" and it occurs when  we have many classes that are related to each other by inheritance.

-->We have two types of polymorphism they are:
   1)compile time polymorphism (or) Method Overloading (or) static polymorphism (or) Early Binding
   2)Run time polymorphism (or) Method Overriding (or) Dynamic Polymorphism (or) Late Binding

Method Overriding (or) Runtime polymorphism:-
----------------------------------------------
why method overriding..?
------------------------
 -->Whenever we are not happy or not satisfying with the parent class functionalities then we will go for method Overriding.

what is Method overriding:-
---------------------------
A Method in parent class is declared with same name , arguments and return type again in child class then that is called as method overriding.


Method Overriding Rules:-
-------------------------
1)Method Signature(name+ arguments but not return type) should be same.
2)Method return type must be same until 1.5 version, afterwards we have co-variant return types.
  Co-variant Return type:-
     -->Method return must be same if it is primitive datatype even after 1.5 version also.
     -->Method return no need to be same if it is object datatype after 1.5 version  we can use co-variant return type.
     -->Covariant return type means , If the  parent class return parent type then our child class can return the parent type or it's child type.
         example:-
             if Parent: Number --> Child : Number or it's sub types(Wrapper Object Datatypes)
3)Method Scope should not be reduced.
4)Parent class private methods , we cannot override them in child classes, if we write the "@Override" annotation or if we are not writing that annotation then the child class is considering it as a different method and there will be no error.
5)parent class final methods, we cannot override them in child classes.
6)Parent class static methods, we cannot override them in child classes when we are using "@Override" annotation but when we are not using that annotation then
  it is considered as Method Hiding.
7)If Parent class throws any exception then child class no need to throws the exception but if the child class throws any Exception then the parent class must throws that exception.
8)Parent abstract class abstract Methods , we must need to override them in Child classes.
9) Parent class regular methods or normal methods we can  override them as abstract methods in abstract child class.


Method Overloading:-
---------------------
-->In  any class, if we have same methods with different types of arguments, then we can call it as Method Overloading.
Best Example:- Println() method from print Stream Class.

Rules for Method Overloading:-
-------------------------------
Rule 1: Method Signature should not be same.
Rule 2: Method Return type is not a part of MOL, whether it is same return type or not.

Benefits of polymorphism:-
==========================
-->Flexibility
-->Loosely Coupling
-->Readability
===============================================================================================================================================================
EXCEPTION HANDLING:-
======================
why we need to Handle Exceptions..?
------------------------------------
 -->For a Graceful or successful termination of a program or Application, we need to Handle Exceptions.

What is Exception?
------------------
-->Exception means a problem which will occur due to "Bad Logics or Bad Data".
-->Exception is an "Unwanted Event" that occurs in a Normal Flow and the program will terminate "abnormally".
-->The Best Example is Corona.
-->Exception is a Pre-defined Class under "Throwable class".
-->"Throwable" is the Parent class of two child classes("Exceptions" and "Errors") in java from java.lang package.
-->We can handle the Exceptions by using below keywords:
      -try
      -catch
      -finally
      -throw
      -throws

What is Error..?
-----------------
-->Error means a problem which will Occur "Due to Lack of Resources".
-->We cannot handle the errors.
-->Example:- Virtual Machine error(OutOfMemoryError, StackOverFlowError).
-->compile time errors and errors are different.(compile time errors-->due to syntactical mistakes, errors-->due to lack of resources.)


Types of Exceptions:
---------------------
There are two types of Exceptions, they are:
 1) Checked Exceptions:-
 ------------------------
   -All "Exception classes" under "Exception class" are checked Exceptions.
   -Any Exceptions which are checked by the compiler at compile time is called as Checked Exceptions.
   -Checked Exceptions will come when we call some specific pre-defined methods and creating an Object of specific classes.
   Examples:-
  -------------
    1)IOException  : when we are calling "creatNewFile()" then we are getting "IOException".
    2)FileNotException : when we are creating Object for "FileReader class" then we are getting "FileNotFoundException".
    3)ClassNotFoundException : when we are calling "Class.forName("Oracle.jdbc.driver.OracleDriver"); then we are getting "ClassNotFoundException".
    4)SQLException : when we are calling "DriverManager.getConnection("URL","username", password"); then we will get "SQL Exception".
    6)EmptyStackException: when we are accessing an empty stack by using "s.peek()" and "s.pop()" then we will get EmptyStackExcpetion.
    6)InterruptedException 
   
  -->throws: throws is the keyword to satisfy the compiler when we are having checked Exceptions.
  -->throw : throw the exceptions Explicitly to the JVM whether it is predefined or user defined Exception.

 2) Unchecked Exceptions.
----------------------------
   -All "Exception classes" under "RunTimeException" class are Unchecked Exceptions.
   -Any Exceptions which are not checked by the compiler at compile time is called as Unchecked Exceptions.

   Examples:-
  ------------
   1)ArithmeticException : If any Number divisible by Zero then we will get "ArithmeticException".
   2)NullPointerException : "null" with any operation is a Null pointer Exception.
   3)IndexOutOfBoundsException 
   4)ArrayIndexOutOfBoundsException : If we give size of an array more than expected then we will get "ArrayIndexOutOfBoundsException".
   5)StringIndexOutOfBoundsException : If we try to access the index which is not available in String then we will get "StringOutOfBoundsException".
   6)InputMismatchException  : If we have declared input as Integer but we are giving String input in console then we will get "InputMissMatchException".

Custom Exceptions or User Defined Exceptions:-
-----------------------------------------------
-->Any class that extends "Exception Class" then we can consider it as Checked Exception.
-->Any Class that extends "RuntimeException" class then we can consider it as Unchecked Exception.

Note:-
---------------
1)Only "try" block is not possible, we must need to provide "catch or finally" blocks.
2)"try" block is to keep problematic code.
3)If there is a problem in  try block then catch block will executes.
4)If there is a problem or not in try block the finally block will always executes.
5)We can have Multiple catch blocks.
6)We cannot have Multiple finally blocks.
7)try ->catch -> finally order is important.
8)The first catch block never be a parent Exception.
9)Only try, only catch, only finally blocks are not possible.
10)Catch with finally  is also not possible without try block. 
11)We cannot write any other statements between "try" and "catch" blocks.
12)We can stop finally block by using "System.exit(0);"
13)Nested try-catch blocks are possible in try block, catch block and finally block also.
===============================================================================================================================================================
FILE IO(File Handling):-
========================
-->The File Io is related to java.io package.
-->The File IO stands for file input output Streams.
-->We are going to understand 11 Predefined classes in File IO.
  ->1)File
  ->2)FileReader
  ->3)FileWriter

  ->4)BufferedReader
  ->5)BufferedWriter
  ->6)PrintWriter

  Serialization:-
--------------------
    
================================================================================================================================================================
COLLECTIONS FRAME WORK OR COLLECTIONS API(Java.util):-
=====================================================
Frameworks:-
-------------
->A system of rules or ideas which help you to decide what to do.

-->There are two Chapters in Collections Frame work they are:
     1)Collections Framework or Collections API is a chapter to discuss Collection Objects.(Interface)
     2)Collections is a utility class.

why Collections..?
-------------------
-->To Structuring the  data in a proper way or organized way, we need to go for concept of Collections Chapter.
-->Representing  Collection of Objects in to a single entity, that entity can be any collection framework Object.

          Array                            vs                          Collections
   ------------------                                           --------------------------
1)Array is a fixed in size , we cannot                     1)Collections are Growable in nature at runtime.
  change it in runtime.
2)Arrays Can allow only homogeneous                        2)Collections can allow both homogeneous and heterogeneous 
  data elements.                                              data elements.
3)Arrays can allow both primitive datatypes                3)Collections can allow only object Data types to store the elements.
  and object data types to store the elements.
4)Memory POV Arrays are not recommended to use.            4)Memory POV Collections are recommended to use.
5)Performance POV Arrays are recommended to use            5)Performance POV Collections are not recommended to use when compare to arrays.
  when we know exact array size.

-->Collections framework Available from java.util package.
-->We are going to learn "15" interfaces in Collections, they are:
   1)Collection
   2)List : ArrayList, LinkedList, Vector, Stack and CopyOnWriteArrayList -->Implemented classes of List Interface.
   3)Queue
   4)Dequeue

   5)Set
   6)SortedSet
   7)NavigableSet
---------------------------------------------
   8)Map
   9)SortedMap
   10)NavigableMap
----------------cursors---------------------
   11)Enumeration
   12)Iterator
   13)ListIterator
   14)Comparable
   15)Comparator
---------------------------------------------
-->All the Collection Interfaces are child interfaces of Collection (root interface).
-->Iterable is the root interface of Collection Interface.

1)Collection:-
--------------
  -The root "Interface" in the Collection Hierarchy.
  -A Collection represents a group of objects, known as its elements.
  -Some Collections allow duplicate elements and other do not.
  -some are ordered and others Unordered.
  -The JDK Does not provide any direct implementations for Collection Interface.
  -It provides implementations of more specific sub Interfaces Like "Set" and "List."

syntax:-
-------------
Collection<Integer> c = new ArrayList<>();
               or
List<Integer> c = new ArrayList<>();
              or
ArrayList<Integer> c = new ArrayList<>();

Collection<String> c1= new ArrayList();

Method Summary:-
----------------
 *    c.add(E e) //boolean, it is a method to add element into collection and expecting element as argument.
 *    c.addAll(Collection<?> c1); //boolean, it is a method to add another Collection to this Collection.
 *    c.clear(); //void , it is a method to clear elements int the enitre Collection.
 *    c.contains(E e); //boolean , it will return true if and only the element contains inthe collection.
 *    c.conatainsAll(Collection<?>c1); //boolean , it will return true if and only if the entire Collection elements
      present in this Collection. 
 *    c.equals(Collection<?> c1); //boolean, It will comapre this Collection "c" with the Specified Collection"c1"
 *    c.isEmpty(); //boolean, it will return true if the Speicfied Collection is Empty.
 *    c.hashCode(); //int return hash code value of this collection.
 *    c.iterator(); //Iterator , Returns an iterator over the elements in this collection.
 *    c.remove(E e); //boolean , It is a method to remove  specified element from the collection.
 *    c.removeAll(Collection<?> c1); //boolean
 *    c.size(); //int , it is a method to return size of the collection.
 *    c.toArray(); //Object[] , it is a method to convert Collection into Array.
 *    String y=x.toArray(new String[0]);
---------------------------------------------------------------------------------------------------------------------------------------------------------
2)List Interface:-
-----------------
-->List Implementation classes are below :
    --ArrayList, LinkedList, Stack, Vector, CopyOnWriteArrayList.
-->List follows "insertion Order".
-->List will allow Duplicate Elements.
-->List can take both homogeneous and heterogeneous data elements.
-->List can allow any number of null values.
-->List is working based on index values.

syntax:-
----------
List<Integer> l = new ArrayList<>();

Method summary:-
----------------
*  l.add(E e); //boolean, It is a method to add element into collection and expecting element as argument.
*  l.add(int index, E e); //void , It is a method to add specific element at the specific index or position.
*  l.addAll(Collection<?> l1); //boolean, It is a method to add another Collection to this Collection.
*  l.addAll(int index, Collection<?> l1); //Inserts all of the elements in the specified collection into this list at the specified position 
*  l.get(int index);   //E, it is a method to retrieve the value in that index.
*  l.indexOf(E e);    //int , it is a method to retrieve the index of the given element.
*  l.clear();  //void , It is a method to clear the enitre collection Object.
*  l.size();   //int , It is a method to find size of the list.
*  l.remove(int index); //E, Removes the element at the specified position in this list .
*  l.removeAll(Collection<?> l1); 
*  l.contains(Object o); //boolean , return true if the specified element contains in this list.
*  l.containsAll(Collection<?> l1); //boolean , return true if this list "l1" contains in the specified list "l".
*  l.iterator(); //Iterator, Returns an iterator over the elements in this List.(hasNext(), next())
*  l.listIterator(); //Iterator, Returns an list iterator over the elements in this list.(hasNext(),next(),previous(),hasPrevious())
*  l.equals(l1);  //boolean
*  l.isEmpty();   //boolean, Return true if there are no elements in this list.
*  l.set(int index, E e); //E , It is a method to change the value at the specified index in this list.
*  l.subList(int fromindex, int toindex);
*  l.lastIndexOf(Object 0);
---------------------------------------------------------------------------------------------------------------------------------------------------------------
ArrayList:-
-----------
-->ArrayList is a Implemented class of List Interface.
-->ArrayList is a resizeable Array.
-->ArrayList can also perform all the similar Operations of List Interface.
-->ArrayList allows duplicate elements and also heterogeneous elements.
-->Insetion order is Preserved.
-->ArrayList is unsynchronized.
-->ArrayList Inital Capicty is 10. (Ic * 3/2).
-->ArrayList class is used to retrive the data from database.

why ArrayList ...  why not Vector..?
--------------------------------------
-->Becuase both the Classes implements Random Access Interface(marker Interface) but ArrayList is not synchronized where as vector is synchronization.Hence
  ArrayList is best option when compared to Vector.(it is little bit of speed)

   ArrayList    vs      Vector
 -------------------------------------------
 * No method in ArrayList is synchronized.
 * Most of the methods in vector are synchronized.

 *At a time Multiple threads are allowed to operate on ArrayList Object and hence it is not thread safe.
 *At a time only one thread is allowed to operate on Vector Object and hence it is thread safe.

 *performace POV ArrayList is recommended to use.
 *performance POV Vector is not recommended to use.

 *Not legacy and 1.2 version.
 *Legacy and 1.o version.

----------------------------------------------------------------------------------------------------------------------------------------------------------------
Linked List:-
--------------
 -->LinkedList is a Implemented class of List Interface.
 -->LinkedList is a resizeable array.
 -->LinkedList can also perfrom all the similar Operations of List Interface.
 -->LinkedList allow Duplicate elements and also hetergeneous elements.
 -->Insertion order is Preserved.
 -->LinkedList is unsynchronized.

 why LinkedList .. why not ArrayList..?
--------------------------------------------
 -->In LinkedList , Insertion and deletion of elements is faster when compare to ArrayList even though they are unsynchronized.

Method Summary of LinkedList:-
-------------------------------
All the methods of List Interace and additionally we have some extra methods they are:

* addFirst(E e); //void, Appends specified element to the beginning of the list.
* addLast(E e);  //void, Appends specified element to the end of the list.
* getFirst();  //E, Returns the first element in the list.
* getLas();    //E, Returns the last element in the list.
* removeFirst(); //E, Removes and returns the First element in the list.
* removeLast(); //E, Removes and returns the last element in the list.


copyOnWriteArryList:-
-------------------------
-->copyOnWriteArrayList is a class from java.util.concurrent package.
-->copyOnWrtieArrayList can also perform all the similar operations of List interface.
-->copyOnWriteArrayList is Fail safe.

why copyOnWriteArrayList..  ... why not ArrayList..?
----------------------------------------------------
-->ArrayList is Fail fast where as copyOnWriteArrayList is Fail safe.
(Fail Fast -->It does not allow modification while iterating, if we do the same then we will get concurrentmodification error)
(Fail Safe -->It allows modification of elements while Iterating.

Method Summary of vector:-
--------------------------
syntax:-
-------
 Vector v = new Vector<>();

1) v.addElement(E e);
2) v.elements(); // Enumeration<?> e (hasMoreElements(), nextElement())
3) v.add(E e);

Stack:-
---------
-->Stack is LIFO(Last in First Out)
-->vector is the parent class of Stack.
synatx:-
--------
Stack<String> s = new Stack<>();
Method Summary:-
---------------
1)s.push(E e); //it is used to add Object into the stack.
2)s.peek();  //Returns the Object which is in the top position
3)s.pop(); //remove the object from Stack
4)s.search(Objec o); //int
5)s.empty(); //boolean , return true if the stack have no objects.
----------------------------------------------------------------------------------------------------------------------------------------------------------------
Set:-
------
 syntax:-
-------------
  Set<?> s = new HashSet<>();
  Set<?> s1 = new LinkedHashSet<>(); //LinkedHashSet is following insertion order.

-->Set will not follow Insertion Order and it follow based on hashCode.
-->Set will not allow Duplicate values.
-->Set will allow null values only once.
-->Set can allow both homogeneous and heterogeneous data elements
-->Set is a Interface. -- HashSet, LinkedHashSet
-->SoretedSet is a  Sub Interface of Set Interface.(TreeSet)
-->NaviagbleSet is a sub Interface of  SortedSet.(TreeSet)
-->The Main intension for going to "Set" Interface is to remove Duplication.
-->The default initial Capacity of  Set is "16" and the load factor is (0.75).
-->The HashSet is Working internally based on "HashMap".
-->"HashSet" is working based on hashCode and "LinkedHashSet" is working based on 'linkedlist".
-->If our frequent Operation is searching then we can go for "HashSet".
-->set Interface and it's sub Interfaces can also perfrom all the similar Operations of List Interface.

SortedSet:-
--------------
SortedSet<?> s2 = new  TreeSet<>();

-->SortedSet follows sorted order.
-->If we pass any null value to the SortedSet or TreeSet then we will get "NullPointerException."
-->SoretedSet is a sub Interface of Set Interface.
-->TreeSet is a implemented class of SortedSet Interface
-->TreeSet allows only Homogeneous data elements.

Method Summary:-
-----------------
* s2.first();
* s2.last();
* s2.tailSet(E e); //Returns elements strictly greater than or equal to the given element.
* s2.headSet(E e);  //Returns elements strictly less than to the given element.
* s2.subSet(E e1, E e2);

NavigableSet:-
----------------
 NavigableSet s = new TreeSet<>();

-->NavigableSet also follows Sorting order.
-->NavigableSet is a sub Interface of SortedSet.
-->TreeSet is a implemented class of NavigableSet and it allows only Homogeneous Elements.
-->If we are trying to pass heterogeneous elements to TreeSet then we will get "ClassCastException".

Method Summary for NavigableSet:-
----------------------------------
*  s.floor(E e);
*  s.ceiling(E e);
*  s.higher(E e);
*  s.lower(E e);

Comparable:-
------------
-->Comparable is a Interface from java.lang package.
-->"compareTo(Object o)" is a abstract method from Comaparable Interface which is expecting an Object as argument and the return type is "int".
--> compares "this" Object with the specified Object for Order.
--> Returns a positive Integer(+1) if this object is greather than the specified Object.
--> Returns a Negative Integer(-1) if this Object is lessthan than the specified Object.
--> Returns Zero , if this Object equals to the Specified Object.

Comparator:-
-------------
-->Comparator is a Interface from java.util package
-->"compare(T o1, T o2)" is a abstract method from comparator Interface which is expecting two arguments and the return type is "int".
-->compares first Object or argument with the Second argument or Object.
-->Returns a positive Integer(+1) if the first argument is greater than second argument.
-->Returns a Negative Integer(-1) if the second argument is less than second argument.
-->Returns Zero if first arguments equals to second argument.

Comparable  vs Comparator:-
---------------------------
* Comparable Interface is used to sort the Objects with Natural Ordering.
* Comparator Interface is used to sort the  attributes of different Objects.

* Comparable Interface compares "this" object with the "specified" Object.
* Comparattor Interface compares two different Objects provided by class.

* Comparable Interface is from java.lang package.
* Comparator Interface is from  java.util package.

* Comparable Interface affect's the Original Class.
* Comparator Interface does not affect the Original class.

* Comparable Interface provides "compareTo()" method to sort the elements.
* Comparator Interface provides "compare()" and "equals()" methods to sort the elements.


Map:-
------
-->Map is a interface from java.util package.
-->Map implemented classes are HashMap, LinkedHashMap, IdentityHashMap, WeakHashMap.
-->Map is for representing key,value pairs.
-->keys cannot be duplicated but values can be duplicated.

HashMap:-
---------
-->HashMap is internally working based on HashTable.
-->HashMap is fail fast and  it is unsynchronized.
-->HashMap is using ".equals()" method to check the keys from map.
-->HashMap Order is not preserved.
-->HashMap Dominates Garbage Collector, where HashMap we used it in cache based Algorithms.
-->HashMap allows one "null" key and any number of "null" values.
-->LinkedHashMap follows insertion Order.

IdentityHashMap:-
----------------
-->IdentityHashMap is a implemented class of Map Interface.
-->IdentityHashMap is using "==" operator to check the keys from map.

WeakHashMap:-
-------------
-->Garbage Collector dominates WeakHashMap, if we want to perform garbage collection on map then we will go for "WeakHashMap".

Map<Integer, String> m = new HashMap<>();

Method Summary:-
----------------
* m.put(key, value); //Returns the previous value associated with key or "null" if there was no mapping for key.
* m.putAll(Map<?,?> m);
* m.get(key); //Returns the value associated with the key.
* m.entrySet(); //Returns the "Set" view of mappings contained in this map.
* m.keySet(); 
* m.values();
* m.size();
* m.containsKey(key); //boolean, Returns true if the key contains in a map.
* m.containsValue(value); //boolean, Returns true if the value contains in a map.
* m.clear();
* m.isEmpty(); //Retruns true if the map is Empty.
* m.remove(Key); 
* m.replace(key, value);
* m.replace(key, oldvalue, newvalue);

//Adding list of elements to the Map.
 char[] c = str.toCharArray();
 for(char ch : c ){
     if(m.containsKey(ch)){
        m.put(ch, m.get(ch)+1);
     }
     else{
        m.put(ch,1);
     }
 }


//Reprsenting the  keySet in a Map
 for(Integer i:m.keySet()){
   System.out.println(i);
 }

//Representing the  values in a Map
  for(String s:m.values()){
    System.out.println(s);
  }

//Pushing array elements in to Map
 for(data_type i : A){
       if(m.contains(i){
         m.put(i, m.get(i)+1);
        }
        else{
          m.put(i,1_;
       }
 }
         
-->Set<Map.Entry<Integer, String>> entries = m.entrySet();
   for(Map.Entry<Integer, String>> entry : entries){
     System.out.println(entry.getKey() +" : "+ entry.getValue());
     //getValue(); //return the value corresponding to this entry.
     //getKey();   //return the key corresponding to this entry.
     //equals(Object o); //compares the specified object with this entry for eqaulity.
     if(entry1.getValue() != null)
     {
        System.out.println(entry1.getValue().equals(entry2.getValue()));
      }

   }

  SortedMap:-
  -------------
  SortedMap<?,?> s = new TreeMap<>();
  -->SortedMap follows sorted order.
  -->TreeMap is a implemented class of SortedMap.
  -->TreeMap only allows Homogeneous Elements.
  -->If we pass any Heterogeneous elements to the TreeMap then we will get "ClassCastException".

  HashMap  vs  HashTable  vs concurrentHashMap
 -----------------------------------------------
  * HashMap is not thread safe because it allows multiple threads to execute at a time.
  * HashTable is thread safe because it allows only one thread to execute at a time.

  *HashMap allows one "null" key and any number of "null" values.
  *HahsTable does not allow any "null" key and "null" values.

  *Peformance pov HashMap is recommended to use.
  *Performance pov HashTable is not recommended to use.

  *HashMap is fail fast.
  *ConcurrentHashMap is fail safe.


 Queue:-
----------

================================================================================================================================================================
COLLECTIONS IS A UILITY CLASS IN JAVA:-
========================================
-->This Collections class provide some generic functionalities to work with Collection.
-->"Collections.sort(list_name); " -->It is used to sort the elements of array or list.
-->"Collections.copy(l1,l2) ;" -->It is used to copy elements from one array to another array. 
-->"Collections.swap(arr,index1,index2);" --">It is used to swap elements of the array.
-->"Collections.reverse(arr);" -->It is used to reverse  elements of the array.
-->"Collections.frequency(arr,ele);"
-->"Collections.max(arr);" -->It is used to find maximum element of the array.
-->"Collections.min(arr);" -->It is used to find minimum element of the array.
-->"Collections.shuffle(arr);"  -->It will rearrange all the elements of the array.
-->"Collections.replaceAll(arr, old_value, new_value);"
-->"Collections.binarySearch(arr,ele);"
-->"Collections.rotate(arr,how_many_rotations);
================================================================================================================================================================
INNER CLASSES:-
----------------
what is Inner class?
----------------------
-->A class Inside a class is called as Inner class.
-->Without Outer class there is no Inner class.
-->The purpose of Inner classe is to complete Temporary Requirements.
There are 4 Types of Inner classes:-
------------------------------------
1) Regular or Named inner Classes
2) Method Inside Inner classes
3) Anonymous Inner classes.
4) Static Inner classes.

=================================================================================================================================================================
MULTI THREADING:-
---------------
Why?
----
->Reducing response time
What is Thread in MT:-
---------------------
->A light weight execution process is called Thread.
->It will execute multiple functionalities in same time.
->Thread is a pre-defined class from java.util.class.
--------------------------------------------------------
MULTI TASKING:-
-------------
->Executing several taska simultaneously is the concept of multitasking or executing multiplt tasks at the same time is called as Multi Tasking.
->Two types:
  1)PBM (Process Based Multittasking) Ex: CPU, Browser
      ->Executing several tasks simaultaneously where each task is a separate independent programme(process) is called PBM.
      ->These are OS level task but not at Programming level.
  2)TBM (Thread Based Multittasking)  Ex: Text editing, spell checking
      ->Executing several tasks simaultaneously where each task is a separate independent programme(process) is called TBM.
      ->TBM is suitable at programmatic level.
----------------------------------------------------------------------------------------------------------------------------------------------
The main important application areas of multithreading are :
--------------------------------------------------------
1) To develop Multimedia Graphics.
2) To implement Video animation.
3) To develop games.
4) To develop a Server.
5) To develop servers and web application servers.
6) When comparing C++ developing multitgreading programs in java is very easy because java provides inbuilt support by providing a RICH API(Thread, ThreadGroup,      Runnable etc..).
----------------------------------------------------------------------------------------------------------------------------------------------------------------


=================================================================================================================================================================
JAVA CHAPTER 1 INTERVIEW QUESTIONS:-
=====================================
-->Why u choose java and what are the features of java?
-->what is the difference c/C++ and java?
-->what is the difference b/w static and dynamic memory allocation?
-->difference b/w class and object?
-->what is the difference b/w source code, byte code , binary code or machine level code?
-->what is the difference static v/s Instance data members?
-->what are the different types of Class loaders?
-->what are the different memory managements in JVM?
-->what is the difference b/w interpreter and JIT?
-->Explain About Garbage Collection how can we achieve this?
-->Explain about main method why need to have in java?
-->Difference between Static Blocks and instance Blocks.
===============================================================================================================================================================
