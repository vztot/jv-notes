# Java Notes

## Purpose of the project
These notes was made for better understanding of java

## Table of contents

### Java Core
- [x] [Java History and Philosophy](#java-history-and-philosophy)
- [x] [Primitives](#primitives)
- [x] [Objects](#objects)
- [x] [Wrappers](#wrappers)
- [x] [Conversions](#conversions)
- [x] [Autoboxing and unboxing](#autoboxing-and-unboxing)
- [x] [Arrays](#arrays)
- [ ] Quick Converting
- [ ] String vs StringBuilder
- [ ] OOP
- [ ] Static Classes, Static Methods, Static Variables
- [ ] Exceptions
- [ ] Abstract Classes vs Interfaces
- [ ] Build Pattern
- [ ] Java NIO vs IO
- [ ] RegEx
- [ ] Cloneable
- [ ] Equals
- [ ] HashCode
- [ ] Generics
- [ ] Wildcard
- [ ] PECS
- [ ] ArrayList
- [ ] LinkedList
- [ ] Immutable class
- [ ] HashMap
- [ ] TreeMap
- [ ] Comparator
- [ ] Iterator
- [ ] Set
- [ ] TreeSet
- [ ] Queue
- [ ] Stack
- [ ] Collection Framework
- [ ] Optional
- [ ] Anonymous class
- [ ] Functional interfaces
- [ ] Lambda
- [ ] Method reference
- [ ] Stream API
- [ ] Iterate and Generate
- [ ] Parallel Streams
- [ ] DateTime API
- [ ] Reflection API
- [ ] Multithreading
- [ ] Synchronized block
- [ ] Deadlock
- [ ] Livelock
- [ ] Volatile
- [ ] Mutex
- [ ] Monitor
- [ ] Semaphore
- [ ] Runnable
- [ ] Callable
- [ ] ExecutorService
- [ ] ForkJoin
- [ ] java.util.concurrent.*
- [ ] Atomics
- [x] [Relevant Java Links](#relevant-java-links)

### Servlets
- [ ] Servlet
- [ ] Server
- [ ] Model, View, Controlled and DAO
- [ ] Tomcat
- [ ] Web.xml
- [ ] JSP
- [ ] Request Dispatcher
- [ ] Http Methods
- [ ] GET
- [ ] POST
- [ ] Http Codes
- [ ] JSTL
- [ ] Security in Web
- [ ] Authentication and Authorization
- [ ] RBAC vs ABAC
- [ ] Cookies
- [ ] Filters
- [ ] HttpSession

### JDBC & SQL
- [ ] SQL vs NoSQL
- [ ] SQL basics
- [ ] JDBC
- [ ] JDBC driver
- [ ] DB connection
- [ ] MySQL connection example
- [ ] Password hashing

### Hibernate
- [ ] JPA
- [ ] ORM
- [ ] What is Hibernate?
- [ ] Session and SessionFactory
- [ ] Entity annotations
- [ ] CriteriaQuery
- [ ] HQL
- [ ] Hibernate.cfg.xml
- [ ] Entity states
- [ ] Relationships
- [ ] Cascade
- [ ] LazyInitializationException
- [ ] Transaction
- [ ] ACID
- [ ] Isolation levels
- [ ] JPA proxy object
- [ ] N+1 problem
- [ ] Cache levels
- [ ] JPA inheritance
- [ ] Transient annotation
- [ ] Annotations

### Spring
- [ ] AoP
- [ ] IoC
- [ ] DI
- [ ] ApplicationContext
- [ ] Beans
- [ ] Bean Lifecycle
- [ ] Autowiring
- [ ] Circular Dependency
- [ ] Primary and Qualifier
- [ ] DataSource configuration
- [ ] Properties file
- [ ] Spring Web MVC
- [ ] View resolver
- [ ] Controller and RestController
- [ ] Bean scope
- [ ] What is REST?
- [ ] REST vs SOAP
- [ ] Spring Security
- [ ] Security Configuration
- [ ] SecurityContext
- [ ] Spring Boot
- [ ] Spring Data
- [ ] Annotations

### Advanced
- [x] [GIT](#git)
- [x] [Maven](#maven)
- [x] [Google Java Style Guide](#google-java-style-guide)
- [ ] Binary operations
- [ ] Big O
- [ ] Basic algorithms in Java
- [ ] JUnit
- [ ] Log4j
- [ ] Lombok
- [ ] TCP vs UDP

### Patterns and Principles
- [ ] PECS
- [ ] DAO
- [ ] CRUD
- [ ] MVP
- [ ] MVC
- [ ] SOLID
- [ ] ACID
- [ ] IoC
- [ ] DI
- [ ] DTO
- [ ] REST
- [ ] SOAP

### Additional environment
- [ ] MySQL Workbench
- [ ] Postman
- [ ] Swagger
- [ ] H2

## Java Core

## java-history-and-philosophy

### History

Java was started as a project called "Oak" by James Gosling in June 1991. Gosling's goals were to implement a virtual machine and a language that had a familiar C-like notation but with greater uniformity and simplicity than C/C++. The first public implementation was Java 1.0 in 1995. It made the promise of "Write Once, Run Anywhere", with free runtimes on popular platforms. It was fairly secure and its security was configurable, allowing for network and file access to be limited. The major web browsers soon incorporated it into their standard configurations in a secure "applet" configuration. popular quickly. New versions for large and small platforms (J2EE and J2ME) soon were designed with the advent of "Java 2". Sun has not announced any plans for a "Java 3".

### Philosophy

There were five primary goals in the creation of the Java language:
1. It should use the object-oriented programming methodology.
2. It should allow the same program to be executed on multiple operating systems.
3. It should contain built-in support for using computer networks.
4. It should be designed to execute code from remote sources securely.
5. It should be easy to use by selecting what was considered the good parts of other object-oriented languages.

## primitives

**They're stored in the stack.**

The eight primitives defined in Java are `int`, `byte`, `short`, `long`, `float`, `double`,
 `boolean`, and `char` – those aren't considered objects and represent raw values:

```java
// integer types
boolean bool = true;        // boolean size is virtual machine dependent
byte b = 127;               // 1 byte; from -128 to 127 
short s = 1123;             // 2 byte; from -32768 to 32767
char c = 65;                // 2 bytes; from -32768 to 32767; is similar to "char c = 'A';" and "char c = 65 + 32;" is similar to "char c = 'a';"  
int i = 2_000_000_000;      // 4 bytes; from -2147483648 to 2147483647; u can use "_" whenever except of ending and begining
long l = 12321312321312L;   // 8 bytes; from -9223372036854775808L to 9223372036854775807L; postfix "L" or "l" mean literals of type long; we use upper-case because of Google Style

// float pointing types
float f = 17.08F;           // 4 bytes; from 1.4e-45f to 3.4e+38f always with "F" or "f" at the end.
double d = 77.99;           // 8 bytes; from 4.9e-324 to 1.7e+308; java double is IEEE 754 standard comliant

// some other notations
int k = 0b111010;           // binary notation
int m = 012;                // octal notation
int n = 0xCAFE;             // hexadecimal notation
long l = 0xCAFE_DEAL;       // hexadecimal with literal
```

## objects

An object is a class instance or an array.

The reference values (often just references) are pointers to these objects, and a
special `null` reference, which refers to no object.

```java
Object object = new Object(); // here "object" is a reference to the Object class instance
int[] arr = new int[1]; // here "arr" is a reference to the int array instance
```

## wrappers

**They're stored in the heap.**

Wrapper classes are objects encapsulating primitive Java types. Each Java primitive has a corresponding wrapper.
Basically, generic classes only work with objects and don't support primitives. As a result, if we want to work with them, we have to convert primitive values into wrapper objects.

Other source says that wrappers was created because data structures in java (ArrayList, HashMap etc.) can store only the objects and plus the object is needed to support synchronization in multithreading.

Wrapper initialization:

```java
Boolean b = true;
Short s = 32_000;
Character c = 'c';
Integer i = 0b00001;
Long l = 12312321211L;
Float f = 1212.2f;
```

## conversions

### Primitive to Primitive Conversions

When we need to convert from a primitive that is simpler or smaller than the destination type, we don't have to use any special notation for that
```java
int myInt = 127;
long myLong = myInt;
```
During widening conversion, the smaller primitive value is placed over a larger container, which means that all the extra space, on the left of the value, is filled with zeros. This may also be used to go from the integer group to the floating point

```java
float myFloat = myLong;
double myDouble = myLong;
```
This is possible because the moving to a wider primitive does not lose any information.

Sometimes we need to fit a value that is larger than the type used in the variable declaration. This may result in information loss since some bytes will have to be discarded.

In this case, we have to explicitly express that we are aware of the situation and we agree with that, by using a cast:


```java
int myInt = (int) myDouble;
byte myByte = (byte) myInt;
```

### Primitive to Wrapper Class Conversions

We can either use constructor or static factory methods to convert a primitive value to an object of a wrapper class

```java
Integer object = new Integer(1);
Integer anotherObject = Integer.valueOf(1);

int a = object.intValue();
int b = anotherObject.intValue();
```

## autoboxing-and-unboxing

**After Java 5**. Autoboxing is the automatic conversion that the Java compiler makes between the
 primitive types and their corresponding object wrapper classes. If the conversion goes the other way, this is called unboxing.
 
 Here is the simplest example of autoboxing:
```java
Character ch = 'a';
```

And another one:

```java
List<Integer> list = new ArrayList<>();
        for (int i = 1; i < 50; i += 2) {
            list.add(i);
        }
```

Thus, the compiler converts the previous code to the following at runtime:

```java
List<Integer> list = new ArrayList<>();
       for (int i = 1; i < 50; i += 2) {
           list.add(Integer.valueOf(i));
       }
```

Converting a primitive value (an int, for example) into an object of the corresponding wrapper class (Integer) is called autoboxing. The Java compiler applies autoboxing when a primitive value is:

* Passed as a parameter to a method that expects an object of the corresponding wrapper class.
* Assigned to a variable of the corresponding wrapper class.

Unboxing example:

```java
public class Unboxing {
 
    public static void main(String[] args) {
 
        Integer i = new Integer(-8);
 
        // 1. Unboxing through method invocation
        int absVal = absoluteValue(i);
        System.out.println("absolute value of " + i + " = " + absVal);
 
        List<Double> ld = new ArrayList<>();
        ld.add(3.1416);    // PI is autoboxed through method invocation.
 
        // 2. Unboxing through assignment
        double phi = ld.get(0);
        System.out.println("phi = " + phi);
    }
 
    public static int absoluteValue(int i) {
        return (i < 0) ? -i : i;
    }
}
```

## arrays
In the Java programming language, arrays are objects, are dynamically
created, and may be assigned to variables of type `Object`. All methods of
class `Object` may be invoked on an array.

An array object contains a number of variables. The number of variables may be
zero, in which case the array is said to be empty. The variables contained in an
array have no names; instead they are referenced by array access expressions that
use non-negative integer index values. These variables are called the components
of the array. If an array has n components, we say n is the length of the array;
the components of the array are referenced using integer indices from 0 to n - 1,
inclusive.

All the components of an array have the same type, called the component type of
the array. If the component type of an array is `T`, then the type of the array itself
is written `T[]`.

The element type of an array may be any type, whether primitive or reference. In
particular:
*  Arrays with an interface type as the element type are allowed.
  An element of such an array may have as its value a null reference or an instance
  of any type that implements the interface.
* Arrays with an `abstract` class type as the element type are allowed.
  An element of such an array may have as its value a null reference or an instance
  of any subclass of the `abstract` class that is not itself `abstract`.

Declarations of Array Variables:
```java
int[] ai;           // array of int
short[][] as;       // array of array of short
short s,            // scalar short
aas[][];            // array of array of short
Object[] ao,        // array of Object
otherAo;            // array of Object
Collection<?>[] ca; // array of Collection of unknown type
```
You can also place the brackets after the array's name:
```java
// this form is discouraged
float anArrayOfFloats[];
```
However, convention discourages this form; the brackets identify the array type and should 
appear with the type designation.

The declarations above do not create array objects. The following are examples of
declarations of array variables that do create array objects:

```java
Exception ae[] = new Exception[3];
Object aao[][] = new Exception[2][3];
int[] factorial = { 1, 1, 2, 6, 24, 120, 720, 5040 };
char ac[] = { 'n', 'o', 't', ' ', 'a', ' ',
              'S', 't', 'r', 'i', 'n', 'g' };
String[] aas = { "array", "of", "String", };
```
The array's `length` is available as a final instance variable `length`.

An attempt to access an array component with a long index value results in a
compile-time error.

All array accesses are checked at run time; an attempt to use an index that
is less than zero or greater than or equal to the length of the array causes an
ArrayIndexOutOfBoundsException to be thrown.

Copying Arrays:

The System class has an arraycopy method that you can use to efficiently
 copy data from one array into another:

```java
class ArrayCopyDemo {
    public static void main(String[] args) {
        char[] copyFrom = { 'd', 'e', 'c', 'a', 'f', 'f', 'e',
			    'i', 'n', 'a', 't', 'e', 'd' };
        char[] copyTo = new char[7];

        System.arraycopy(copyFrom, 2, copyTo, 0, 7);
        System.out.println(new String(copyTo));
    }
}
```
Some other useful operations provided by methods in the java.util.Arrays class, are:

* Searching an array for a specific value to get the index at which it is placed 
(the binarySearch method).
* Comparing two arrays to determine if they are equal or not (the equals method).
* Filling an array to place a specific value at each index (the fill method).
* Sorting an array into ascending order. This can be done either sequentially, 
using the sort method, or concurrently, using the parallelSort method introduced in Java SE 8.
 Parallel sorting of large arrays on multiprocessor systems is faster than sequential array sorting.
 
 ## Advanced
 
 ### relevant-java-links
 [Java Docs 11](https://docs.oracle.com/en/java/javase/11/docs/api/index.html)
 
 [Java Language and Virtual Machine Specifications](https://docs.oracle.com/javase/specs/)
 
 [Oracle Java Downloads](https://www.oracle.com/java/technologies/javase-downloads.html)
 
 [sdkman.io](https://sdkman.io/)
 
 [jenkov.com](http://tutorials.jenkov.com/)
 
 [baeldung.com](https://www.baeldung.com/)
 
 
 ### git
 [GIT Manual](https://git.github.io/htmldocs/git.html)
 
 [GIT Install](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
 
 [.md Guide](https://guides.github.com/features/mastering-markdown/)
 
 File **.gitignore**:
 
 ```
 .idea/*
 target/*
 out/*
 logs/*
 *.iml
 ```
 
 Relevant git commands: 
 
 |command|description|
 |---|---|
 |`git --version`|prints git version|
 |`git init`|add git to a project|
 |`git add .`|add all files of a project to git|
 |`git remote add reponame https://repository.com/address.git`|add new tracked repo|
 |`git remote`|prints set of tracked repos|
 |`git checkout -b branchname`|checkout to new branch "branchname"|
 |`git commit -am "commit msg"`|make a commit|
 |`git push reponame branchname`|push to tracked repo|
 |`git rm -r --cached`|remove git|
 
 ### maven
 
 [Maven Manual](https://maven.apache.org/guides/index.html)
 
 [Maven Install](https://www.baeldung.com/install-maven-on-windows-linux-mac)
 
 Relevant maven commands: 
 
 ```
 mvn --version
 mvn clear
 mvn package
 ```
 
 ### google-java-style-guide
 [Manual](https://google.github.io/styleguide/javaguide.html)
