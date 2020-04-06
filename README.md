# Java Notes

This topic will consist of most relevant java notes imho.

## TODO List

- [x] Relevant Java Links
- [x] GIT
- [x] Maven
- [x] Google Java Style Guide
- [x] Java History and Philosophy
- [ ] Primitives and wrappers. Autoboxing
- [ ] Quick type converting
- [ ] String vs StringBuilder
- [ ] OOP
- [ ] Exceptions
- [ ] Abstract Classes vs Interfaces
- [ ] Build Pattern
- [ ] Cloneable
- [ ] Java NIO vs. IO
- [ ] Equals
- [ ] HashCode
- [ ] RegEx
- [ ] Generics
- [ ] And many others...

## Relevant Java Links

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

**History**

Java was started as a project called "Oak" by James Gosling in June 1991. Gosling's goals were to implement a virtual machine and a language that had a familiar C-like notation but with greater uniformity and simplicity than C/C++. The first public implementation was Java 1.0 in 1995. It made the promise of "Write Once, Run Anywhere", with free runtimes on popular platforms. It was fairly secure and its security was configurable, allowing for network and file access to be limited. The major web browsers soon incorporated it into their standard configurations in a secure "applet" configuration. popular quickly. New versions for large and small platforms (J2EE and J2ME) soon were designed with the advent of "Java 2". Sun has not announced any plans for a "Java 3".

**Philosophy**

There were five primary goals in the creation of the Java language:
1. It should use the object-oriented programming methodology.
2. It should allow the same program to be executed on multiple operating systems.
3. It should contain built-in support for using computer networks.
4. It should be designed to execute code from remote sources securely.
5. It should be easy to use by selecting what was considered the good parts of other object-oriented languages.

## Primitives and wrappers. Autoboxing

**Primitives**

```java
// integer types
byte b = 127;               // 1 byte; from -128 to 127 
short s = 1123;             // 2 byte; from -32768 to 32767
char c = 65;                // 2 bytes; from -32768 to 32767; is similar to "char c = 'A';" and "char c = 65 + 32;" is similar to "char c = 'a';"  
int i = 2_000_000_000;      // 4 bytes; from -2147483648 to 2147483647; u can use "_" whenever except of ending and begining
long l = 12321312321312L;   // 8 bytes; from -9223372036854775808L to 9223372036854775807L;i postfix "L" or "l" mean literals of type long; we use upper-case because of Google Style

// float pointing types
float f = 17.08F            // 4 bytes; from 1.4e-45f to 3.4e+38f
double d = 77.99            // 8 bytes; from 4.9e-324 to 1.7e+308
```