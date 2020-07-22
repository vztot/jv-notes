# Java Notes

## Purpose of the project
These notes was made for better understanding of java

## Table of contents

### Java Core
- [x] [Java History and Philosophy](#java-history-and-philosophy)
- [x] [OOP](#oop)
- [ ] [JVM JRE JDK](#jvm-jre-jdk)
- [x] [Primitives](#primitives)
- [ ] [Binary operations](#binary-operations)
- [x] [Objects](#objects)
- [x] [Object class methods](#object-class-methods)
- [x] [Wrappers](#wrappers)
- [x] [Conversions](#conversions)
- [x] [Autoboxing and unboxing](#autoboxing-and-unboxing)
- [x] [Arrays](#arrays)
- [x] [Quick Array To List List To Array Converting](#quick-array-to-list-list-to-array-converting)
- [x] [String vs StringBuilder vs StringBuffer](#string-vs-stringbuilder-vs-stringbuffer)
- [x] [String concatenation](#string-concatenation)
- [x] [String pool](#string-pool)
- [ ] [Integer pool](#integer-pool)
- [ ] [Memory heap](#memory-heap)
- [ ] [Memory stack](#memory-stack)
- [ ] [JMM](#jmm)
- [ ] [Garbage collector](#garbage-collector)
- [ ] [Static Classes](#static-classes)
- [ ] [Static Methods](#static-methods)
- [ ] [Static Variables](#static-variables)
- [ ] [Exceptions](#exceptions)
- [ ] [Closeable](#closeable)
- [ ] [Abstract Class](#abstract-classes)
- [ ] [Interface](#interface)
- [ ] [Java NIO vs IO](#java-nio-vs-io)
- [ ] [Object Class](#object-class)
- [ ] [RegEx](#regex)
- [ ] [Cloneable](#clonable)
- [x] [Equals](#equals)
- [x] [HashCode](#hashcode)
- [ ] [Generics](#generics)
- [ ] [Wildcard](#wildcard)
- [ ] [Collection Framework](#)
- [ ] [ArrayList](#array-list)
- [ ] [LinkedList](#linked-list)
- [ ] [Stateless class](#stateless-class)
- [ ] [Immutable class](#immutable-class)
- [ ] [Map](#map)
- [ ] [HashMap](#hash-map)
- [ ] [Comparator](#comparator)
- [ ] [Iterator](#iterator)
- [ ] [TreeMap](#tree-map)
- [ ] [Set](#set)
- [ ] [TreeSet](#tree-set)
- [ ] [HashSet](#hash-set)
- [ ] [LinkedHashSet](#linked-hash-set)
- [ ] [Queue](#queue)
- [ ] [Dequeue](#queue)
- [ ] [Stack](#stack)
- [ ] [Optional](#optional)
- [ ] [Anonymous class](#anonymous-class)
- [ ] [Functional interface](#functional-interface)
- [ ] [Lambda](#lambda)
- [ ] [Method reference](#method-reference)
- [ ] [Stream API](#stream-api)
- [ ] [Iterate and Generate](#iterate-and-generate)
- [ ] [Parallel Streams](#parallel-streams)
- [ ] [DateTime API](#date-time-api)
- [ ] [Reflection API](#reflection-api)
- [ ] [Multithreading](#multithreading)
- [ ] [Volatile](#volatile)
- [ ] [Synchronized keyword](#synchronized-keyword)
- [ ] [Synchronized block](#synchronized-block)
- [ ] [Deadlock](#deadlock)
- [ ] [Livelock](#livelock)
- [ ] [Mutex](#mutx)
- [ ] [Monitor](#monitor)
- [ ] [Semaphore](#semaphore)
- [ ] [Runnable](#runnable)
- [ ] [Callable](#callable)
- [ ] [ExecutorService](#executor-service)
- [ ] [ForkJoin](#fork-join)
- [ ] [Concurrent API](#concurrent-api)
- [ ] [Atomics](#atomics)
- [x] [Relevant Java Links](#relevant-java-links)

### Servlets
- [ ] [Servlet](#servlet)
- [ ] [Server](#server)
- [ ] [TCP vs UDP](#tcp-vs-udp)
- [ ] [Tomcat](#tomcat)
- [ ] [Web.xml](#web-xml)
- [ ] [JSP](#jsp)
- [ ] [Request Dispatcher](#request-dispatcher)
- [ ] [Http Methods](#http-methods)
- [ ] [GET request](#get-request)
- [ ] [POST request](#post-request)
- [ ] [Http Codes](#http-codes)
- [ ] [JSTL](#jstl)
- [ ] [Security in Web](#security-in-web)
- [ ] [Authentication and Authorization](#authentication-vs-authorization)
- [ ] [RBAC vs ABAC](#rbac-vs-abac)
- [ ] [Cookies](#cookies)
- [ ] [Filters](#filters)
- [ ] [HttpSession](#http-session)

### JDBC & SQL
- [ ] [SQL vs NoSQL](#sql-vs-no-sql)
- [ ] [SQL constrains](#constrains)
- [ ] [SQL basics](#sql-basics)
- [ ] [JDBC](#jdbc)
- [ ] [JDBC driver](#jdbc-driver)
- [ ] [DB connection](#db-connection)
- [ ] [MySQL connection example](#mysql-connection-example)
- [ ] [Password hashing](#password-hashing)

### Hibernate
- [ ] [JPA](#jpa)
- [ ] [ORM](#orm)
- [ ] [What is Hibernate?](#what-is-hibernate)
- [ ] [Session and SessionFactory](#session-vs-session-factory)
- [ ] [Entity states](#entity-states)
- [ ] [HQL](#hql)
- [ ] [CriteriaQuery](#criteria-query)
- [ ] [Hibernate.cfg.xml](#hibernate-cfg-xml)
- [ ] [Entity relations](#entity-relations)
- [ ] [Entity cascades](#entity-cascades)
- [ ] [LazyInitializationException](#lazy-initialization-exception)
- [ ] [Transaction](#transaction)
- [ ] [Isolation levels](#isolation-levels)
- [ ] [Read phenomena](#read-phenomena)
- [ ] [N+1 problem](#n-plus-one-phenomena)
- [ ] [JPA proxy object](#jpa-proxy-object)
- [ ] [Cache levels](#cache-levels)
- [ ] [JPA inheritance](#jpa-inheritance)
- [ ] [Hibernate annotations cheatsheet](#hibernate-annotations-cheatsheet)

### Spring
- [ ] [What is Spring](#what-is-spring)
- [ ] [ApplicationContext](#application-context)
- [ ] [Beans](#beans)
- [ ] [Bean Lifecycle](#bean-lifecycle)
- [ ] [Bean scope](#bean-scope)
- [ ] [Autowiring](#autowiring)
- [ ] [Circular Dependency](#circular-dependency)
- [ ] [Primary and Qualifier](#primary-and-qualifier)
- [ ] [DataSource configuration](#datasource-configuration)
- [ ] [Properties file](#properties-file)
- [ ] [Spring Web MVC](#spring-web-mvc)
- [ ] [View resolver](#view-resolver)
- [ ] [Controller and RestController](#controller-and-rest-controller)
- [ ] [What is REST?](#what-is-rest)
- [ ] [Spring Security](#spring-security)
- [ ] [Security Configuration](#security-configuration)
- [ ] [SecurityContext](#security-context)
- [ ] [UserDetails](#user-details)
- [ ] [Spring Boot](#spring-boot)
- [ ] [Spring Data](#spring-data)
- [ ] [Spring annotations cheatsheet](#spring-annotations-cheatsheet)

### Algorithms
- [ ] [Big O notation](#big-o-notation)
- [ ] [Java data structures complexity](#java-data-structures-complexity)
- [ ] [Binary Search](#binary-search)
- [ ] [Bubble Sort](#buble-sort)
- [ ] [Insertion Sort](#insertion-sort)
- [ ] [Selection Sort](#selection-sort)
- [ ] [Merge Sort](#merge-sort)
- [ ] [Quick Sort](#quick-sort)

### Patterns
- [ ] [Singleton](#singleton)
- [ ] [Abstract factory](#abstract-factory)
- [ ] [Builder](#builder)
- [ ] [Facade](#facade)
- [ ] [Proxy](#proxy)
- [ ] [Command](#command)
- [ ] [Strategy](#strategy)

### Principles
- [ ] [PECS](#pecs)
- [ ] [MVC](#mvc)
- [ ] [DAO](#dao)
- [ ] [CRUD](#crud)
- [ ] [MVP](#mvp)
- [ ] [SOLID](#solid)
- [ ] [ACID](#acid)
- [ ] [AOP](#aop)
- [ ] [IoC](#ioc)
- [ ] [DI](#di)
- [ ] [REST](#rest)
- [ ] [SOAP](#soap)
- [ ] [DTO](#dto)

### Frameworks and libs
- [ ] [JUnit](#junit)
- [ ] [Log4j](#log4j)
- [ ] [Lombok](#lombok)
- [ ] [Swagger](#swagger)
- [ ] [H2](#h2)

### Environment
- [x] [GIT](#git)
- [x] [Maven](#maven)
- [ ] [MySQL Workbench](#mysql-workbench)
- [ ] [Postman](#postman)
- [ ] [Travis](#travis)
- [ ] [SonarQube](#sonarqube)
- [ ] [Heroku](#heroku)
- [ ] [Docker](#docker)

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

## oop
### Fundamentals
Object-oriented programming is a programming paradigm where everything is represented as an object.

### What Are Objects?
An object is an entity that has states and behaviors.

### What Are Classes?
A class is a template or blueprint from which objects are created.
Classes define states as instance variables and behaviors as instance methods.

### Principles of object-oriented programming

- Encapsulation
- Inheritance
- Abstraction
- Polymorphism

### Encapsulation
Encapsulation is a process of wrapping code and data together into a single unit.

### Inheritance
Inheritance is a mechanism in which one object acquires all the states and behaviors of 
a parent object.

### Abstraction
Abstraction is a process of hiding the implementation details and showing only
functionality to the user.


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

##object-class-methods

|Modifier and Type|Method|Description|
 |---|---|---|
 |protected Object|clone()|Creates and returns a copy of this object.|
 |boolean|equals​(Object obj)|Indicates whether some other object is "equal to" this one.|
 |protected void|finalize()|**Deprecated.** The finalization mechanism is inherently problematic.|
 |Class<?>|getClass()|Returns the runtime class of this Object.|
 |int|hashCode()|Returns a hash code value for the object.|
 |void|notify()|Wakes up a single thread that is waiting on this object's monitor.|
 |void|notifyAll()|Wakes up all threads that are waiting on this object's monitor.|
 |String|toString()|Returns a string representation of the object.|
 |void|wait()|Causes the current thread to wait until it is awakened, typically by being notified or interrupted|
 |void|wait​(long timeoutMillis)|Causes the current thread to wait until it is awakened, typically by being notified or interrupted, or until a certain amount of real time has elapsed.|
 |void|wait​(long timeoutMillis, int nanos)|Causes the current thread to wait until it is awakened, typically by being notified or interrupted, or until a certain amount of real time has elapsed.|

 **Question**: What methods object class have?
 
 **Answer**: wait, notify, notifyAll, toString, getClass, finalize, clone, equals, hashCode
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
 primitive types and their corresponding object wrapper classes. If the conversion goes the other 
 way, this is called unboxing.
 
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

Converting a primitive value (an int, for example) into an object of the corresponding wrapper
 class (Integer) is called autoboxing. The Java compiler applies autoboxing when a primitive 
 value is:

* Passed as a parameter to a method that expects an object of the corresponding wrapper class.
* Assigned to a variable of the corresponding wrapper class.

Unboxing example:

```java
List<Double> list = new ArrayList<>();
list.add(3.1416);
double val = list.get(0);
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
*  Arrays with an `interface` type as the element type are allowed.
  An element of such an array may have as its value a null reference or an instance
  of any type that implements the interface.
* Arrays with an `abstract` class type as the element type are allowed.
  An element of such an array may have as its value a null reference or an instance
  of any subclass of the abstract class that is not itself abstract.

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
 
 ## quick-array-to-list-list-to-array-converting
 
int[] -> List\<Integer>
```java
        int[] arr = {1, 2, 3};
        List<Integer> list = Arrays.stream(arr)
                .boxed()
                .collect(Collectors.toList());
```
 
List\<Integer> -> int[]
 ```java
        List<Integer> list = Arrays.asList(1,2,3);
        int[] arr = list.stream()
                .mapToInt(i -> i)
                .toArray();
 ```

Object[] -> List\<Object>
```java
        String[] strings = {"a", "b", "c"};
        List<String> list = Arrays.asList(strings);
```

List\<Object> -> Object[]
 ```java
        List<String> list = Arrays.asList("a", "b", "c");
        String[] arr = list.toArray(new String[]{});
 ```

## string-vs-stringBuilder-vs-stringBuffer

### Differences between String and StringBuilder
The main difference between `String` and `StringBuilder` is `String` is **immutable** while 
`StringBuilder` is **mutable** means you can modify a `StringBuilder` object once you created it 
without creating any new object. This mutable property makes `StringBuilder` an ideal choice 
for dealing with Strings in Java.

### Differences between StringBuffer and StringBuilder
`StringBuilder` provides an API compatible with `StringBuffer`, but with no guarantee of 
synchronization. `StringBuffer` is a thread-safe, mutable sequence of characters. `StringBuilder` 
class is designed for use as a drop-in replacement for `StringBuffer` in places where the string
buffer was being used by a single thread (as is generally the case). Where possible, it is
recommended that `StringBuilder` class be use in preference to `StringBuffer` as it will be
faster under most implementations.

### Performance example

```java
public class Main {
    public static final int LOOPS = 100000;

    public static void main(String[] args) {
        String string = "";
        long t1 = System.currentTimeMillis();
        for (int i = 0; i < LOOPS; i++) {
            string += "j";
        }
        long t2 = System.currentTimeMillis();
        StringBuilder sb = new StringBuilder();
        for (int i = 0; i < LOOPS; i++) {
            sb.append("j");
        }
        long t3 = System.currentTimeMillis();
        System.out.println(string.length());
        System.out.println(sb.toString().length());
        System.out.println("String concatenation (milliseconds): " + (t2 - t1));
        System.out.println("StringBuilder append (milliseconds): " + (t3 - t2));
    }
}
```

Result of execution: 

```
100000
100000
String concatenation (milliseconds): 913
StringBuilder append (milliseconds): 3
```

### Concatenation in runtime

**Question.** Given the 2 toString() implementations below, which one is preferred:

```java
public String toString(){
    return "{a:"+ a + ", b:" + b + ", c: " + c +"}";
}
```

or 

```java
public String toString(){
    StringBuilder sb = new StringBuilder(100);
    return sb.append("{a:").append(a)
          .append(", b:").append(b)
          .append(", c:").append(c)
          .append("}")
          .toString();
}
```

**Answer.** Version 1 is preferable because it is shorter and the compiler will in fact turn it into
version 2 - no performance difference whatsoever.

>An implementation may choose to perform conversion and concatenation in one step to avoid 
>creating and then discarding an intermediate String object. To increase the performance of 
>repeated string concatenation, a Java compiler may use the StringBuffer class or a similar 
>technique to reduce the number of intermediate String objects that are created by evaluation 
>of an expression.

[link](https://docs.oracle.com/javase/specs/jls/se8/html/jls-15.html#jls-15.18.1)

## string-concatenation
Let's look at the next code:
```java
class Test {
    public static void main(String[] args) {
        String hello = "Hello", lo = "lo";

        System.out.println(hello == "Hello");
        System.out.println(Other.hello == hello);
        System.out.println(hello == ("Hel" + "lo"));
        System.out.println(hello == ("Hel" + lo));
        System.out.println(hello == ("Hel" + lo).intern());
    }
}
class Other {
    static String hello = "Hello";
}

```

It will display next result:

```
true  // both strings have same reference because of string pool
true  // same here
true  // concatenation "Hel" + "lo" was made during compilation, so this is similar to first case
false // concatenation made during runtime so ("Hel" + lo) is a new Object and it is not in the pool
true  // same as previous case but .intern() push this string into string pool during runtime
```

## string-pool

String Pool — the special memory region where Strings are stored by the JVM.

Thanks to the immutability of Strings in Java, the JVM can optimize the amount of memory allocated 
for them by storing only one copy of each literal String in the pool. This process is called
 interning.
 
Let's execute next code:
```java
class Test {
    public static void main(String[] args) {
        String hello = "Hello";
        System.out.println(ObjectUtils.identityToString(hello));
        System.out.println(ObjectUtils.identityToString("Hello"));
    }
}
```

Result of execution:
```
java.lang.String@43a25848
java.lang.String@43a25848
```

As we can see both strings have same reference. It's because "Hello" is in the pool of
 strings.
 
 Let's execute another code:
 ```java
class Test {
    public static void main(String[] args) {
        String hello = new String("Hello");
        System.out.println(ObjectUtils.identityToString(hello));
        System.out.println(ObjectUtils.identityToString("Hello"));
    }
}
```
Result of execution:

```
java.lang.String@43a25848
java.lang.String@3ac3fd8b
```

 References are different because string object is created during runtime.
 
## equals

Default implementation (in Object class):

```java
    public boolean equals(Object obj) {
        return (this == obj);
    }
```

Rules of overwriting:
 1. Reflection:
```java
    if (this == object) {
        return true;
    }
```
 2. Null check:
```java
    if (object == null) {
        return false;
    }
```
 3. Symmetric:
```
    if a.equals(b) is true then b.equals(a) must be true.
```
 4. Transitive:
```
    if a.equals(b) and b.equals(c) is true then c.equals(a) must be true.
```
 5. Consistent:
```
    multiply invocations of equals() method must return the same value 
    untill any of properties are modified.
```
 ## hashcode
 
 Contract between equals and hashCode:
 1. If two objects are equal, than they must have same hash code.
 2. If two objects have the same hash code, they may or may not be equal.
 3. If two objects have different hash codes, they must not be equal.
 4. Same object should return same shashcode until any of properties are modified.
 
 ## advanced
 
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
