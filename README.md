# Java Notes

This notes was made for better understanding 

## TODO List

- [ ] Anchor Navigation For This Document
- [x] Relevant Java Links
- [x] GIT
- [x] Maven
- [x] Google Java Style Guide
- [x] Java History and Philosophy
- [ ] Primitives and wrappers. Autoboxing
- [ ] Arrays
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
- [ ] Set
- [ ] TreeSet
- [ ] Queue
- [ ] Stack
- [ ] Collection Framework
- [ ] To be continue...

## Relevant Java Links

[Java Docs 11](https://docs.oracle.com/en/java/javase/11/docs/api/index.html)

[Java Language and Virtual Machine Specifications](https://docs.oracle.com/javase/specs/)

[Oracle Java Downloads](https://www.oracle.com/java/technologies/javase-downloads.html)

[sdkman.io](https://sdkman.io/)

[jenkov.com](http://tutorials.jenkov.com/)

[baeldung.com](https://www.baeldung.com/)

## GIT

[GIT Manual](https://git.github.io/htmldocs/git.html)

[GIT Install](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

[.md Guide](https://guides.github.com/features/mastering-markdown/)

File **.gitignore**:

```
.idea/*
target/*
*.iml
```

Relevant git commands: 

```
git --version
git remote
git remote add reponame https://repository.com/address.git
git checkout -b branchname
git commit -am "commit msg"
git push reponame branchname
git add .
git rm -r --cached
```

## Maven

[Maven Manual](https://maven.apache.org/guides/index.html)

[Maven Install](https://www.baeldung.com/install-maven-on-windows-linux-mac)

Relevant maven commands: 

```
mvn --version
mvn clear
mvn package
```

## Google Java Style Guide

[Manual](https://google.github.io/styleguide/javaguide.html)

## Java History and Philosophy

### History

Java was started as a project called "Oak" by James Gosling in June 1991. Gosling's goals were to implement a virtual machine and a language that had a familiar C-like notation but with greater uniformity and simplicity than C/C++. The first public implementation was Java 1.0 in 1995. It made the promise of "Write Once, Run Anywhere", with free runtimes on popular platforms. It was fairly secure and its security was configurable, allowing for network and file access to be limited. The major web browsers soon incorporated it into their standard configurations in a secure "applet" configuration. popular quickly. New versions for large and small platforms (J2EE and J2ME) soon were designed with the advent of "Java 2". Sun has not announced any plans for a "Java 3".

### Philosophy

There were five primary goals in the creation of the Java language:
1. It should use the object-oriented programming methodology.
2. It should allow the same program to be executed on multiple operating systems.
3. It should contain built-in support for using computer networks.
4. It should be designed to execute code from remote sources securely.
5. It should be easy to use by selecting what was considered the good parts of other object-oriented languages.

## Primitives and wrappers. Autoboxing

### Primitives

**They're stored on the stack.**

The eight primitives defined in Java are int, byte, short, long, float, double, boolean, and char – those aren't considered objects and represent raw values:


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
int n = 0xCAFE_DEAL;        // hexadecimal with literal
```

### Wrappers

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


### Primitive to Wrapper Class Conversion

We can either use constructor or static factory methods to convert a primitive value to an object of a wrapper class

```java
Integer object = new Integer(1);
Integer anotherObject = Integer.valueOf(1);

int a = object.intValue();
int b = anotherObject.intValue();
```

### Autoboxing and Unboxing

**After Java 5**, this conversion can be done automatically by using features called autoboxing and unboxing.