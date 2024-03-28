# Java Programming Guide

## Introduction

Java is a high-level, object-oriented programming language developed by Sun Microsystems (now owned by Oracle Corporation). It is widely used for developing desktop, web, and mobile applications. This guide aims to provide an overview of Java programming concepts and syntax.

## Getting Started

To start programming in Java, you need to set up your development environment. Follow these steps:

1. **Install Java Development Kit (JDK)**: Download and install the JDK from the official Oracle website.

2. **Set up Environment Variables**: Set the `JAVA_HOME` environment variable to the directory where the JDK is installed.

3. **Install an Integrated Development Environment (IDE)**: Choose an IDE such as Eclipse, IntelliJ IDEA, or NetBeans for Java development.

4. **Write Your First Java Program**: Create a file with a `.java` extension, write your Java code, and compile it using the `javac` command.

## Basic Syntax

### Comments

```java
// This is a single-line comment

/*
This is a
multi-line
comment
*/
```
```java
int num = 10; // integer
double decimalNum = 10.5; // double
char letter = 'A'; // character
String name = "Java"; // String
```

### Control Flow Statements

#### If-Else Statement

```java
int num = 10;
if (num > 0) {
    System.out.println("Number is positive");
} else {
    System.out.println("Number is negative");
}
```

### Switch Statement
```java
char grade = 'A';
switch (grade) {
    case 'A':
        System.out.println("Excellent");
        break;
    case 'B':
        System.out.println("Good");
        break;
    case 'C':
        System.out.println("Fair");
        break;
    default:
        System.out.println("Needs Improvement");
}
```

### Loops

## While Loop
```java
int i = 0;
while (i < 5) {
    System.out.println(i);
    i++;
}
```
## For Loop
```java
for (int i = 0; i < 5; i++) {
    System.out.println(i);
}
```

## Enhanced For Loop (For-Each)
```java
int[] numbers = {1, 2, 3, 4, 5};
for (int num : numbers) {
    System.out.println(num);
}
```

## Methods
```java
public class MyClass {
    public static void main(String[] args) {
        int result = add(5, 3);
        System.out.println("Result: " + result);
    }

    public static int add(int a, int b) {
        return a + b;
    }
}
```

## Classes and Objects
```java
public class Car {
    String brand;
    String model;
    int year;

    public Car(String brand, String model, int year) {
        this.brand = brand;
        this.model = model;
        this.year = year;
    }

    public void displayInfo() {
        System.out.println("Brand: " + brand + ", Model: " + model + ", Year: " + year);
    }
}
```

```java
public class Main {
    public static void main(String[] args) {
        Car myCar = new Car("Toyota", "Camry", 2022);
        myCar.displayInfo();
    }
}
```
## Exception Handling
```java
try {
    int result = 10 / 0;
} catch (ArithmeticException e) {
    System.out.println("Error: " + e.getMessage());
}
```
