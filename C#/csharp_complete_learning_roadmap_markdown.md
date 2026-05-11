# Complete C# Learning Guide

## 1. Introduction to C#

- What is C#
- History of C#
- .NET Ecosystem
- C# vs .NET
- CLR (Common Language Runtime)
- CTS (Common Type System)
- CLS (Common Language Specification)
- IL (Intermediate Language)
- JIT Compiler
- Managed vs Unmanaged Code
- Assemblies and Metadata

---

# 2. Setting Up Environment

- Install Visual Studio
- Install .NET SDK
- Using VS Code for C#
- Create First Console App
- Build and Run Applications
- Debugging Basics
- NuGet Package Manager

---

# 3. C# Program Structure

```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Hello World");
    }
}
```

Topics:

- Namespace
- Class
- Main Method
- Statements
- Comments
- Entry Point

---

# 4. Variables and Data Types

## Value Types

Stored directly in memory.

### Integer Types

```csharp
byte
sbyte
short
ushort
int
uint
long
ulong
```

### Floating Point Types

```csharp
float
double
decimal
```

### Other Value Types

```csharp
char
bool
struct
enum
```

## Reference Types

Stored as references to memory locations.

```csharp
string
object
class
interface
array
delegate
record
```

## Nullable Types

```csharp
int?
bool?
DateTime?
```

## var Keyword

```csharp
var name = "John";
```

## Dynamic Type

```csharp
dynamic value = 10;
```

---

# 5. Type Conversion

## Implicit Conversion

```csharp
int a = 10;
double b = a;
```

## Explicit Conversion (Casting)

```csharp
double a = 10.5;
int b = (int)a;
```

## Parse Methods

```csharp
int.Parse()
double.Parse()
```

## Convert Class

```csharp
Convert.ToInt32()
Convert.ToDouble()
```

## TryParse

```csharp
int.TryParse()
```

---

# 6. Operators

## Arithmetic Operators

```csharp
+
-
*
/
%
```

## Comparison Operators

```csharp
==
!=
>
<
>=
<=
```

## Logical Operators

```csharp
&&
||
!
```

## Assignment Operators

```csharp
=
+=
-=
*=
/=
```

## Unary Operators

```csharp
++
--
```

## Null Operators

```csharp
??
?.
??=
```

## Bitwise Operators

```csharp
&
|
^
~
<<
>>
```

---

# 7. Control Statements

## if Statement

```csharp
if(condition)
{
}
```

## if else

```csharp
if(condition)
{
}
else
{
}
```

## switch Statement

```csharp
switch(value)
{
    case 1:
        break;
}
```

## Loops

### for Loop

```csharp
for(int i = 0; i < 5; i++)
{
}
```

### while Loop

```csharp
while(condition)
{
}
```

### do while Loop

```csharp
do
{
} while(condition);
```

### foreach Loop

```csharp
foreach(var item in items)
{
}
```

## break and continue

---

# 8. Methods

## Creating Methods

```csharp
void Print()
{
}
```

## Parameters

- Value Parameters
- Reference Parameters
- Optional Parameters
- Named Parameters

## ref Keyword

```csharp
ref
```

## out Keyword

```csharp
out
```

## params Keyword

```csharp
params
```

## Method Overloading

## Recursion

---

# 9. Arrays and Collections

## Arrays

```csharp
int[] numbers = {1,2,3};
```

## Multidimensional Arrays

## Jagged Arrays

## Collections

### List

```csharp
List<int>
```

### Dictionary

```csharp
Dictionary<int,string>
```

### HashSet

```csharp
HashSet<int>
```

### Queue

```csharp
Queue<int>
```

### Stack

```csharp
Stack<int>
```

## IEnumerable

## ICollection

## Generic Collections

---

# 10. Object-Oriented Programming (OOP)

## Classes and Objects

## Constructors

- Default Constructor
- Parameterized Constructor
- Static Constructor
- Copy Constructor

## this Keyword

## Access Modifiers

```csharp
public
private
protected
internal
protected internal
private protected
```

## Encapsulation

## Properties

```csharp
get
set
init
```

## Inheritance

```csharp
class Child : Parent
```

## Polymorphism

- Method Overloading
- Method Overriding

## virtual Keyword

## override Keyword

## abstract Classes

## Interfaces

```csharp
interface
```

## Sealed Classes

## Static Classes

## Partial Classes

## Records

---

# 11. Strings

## String Basics

## String Methods

```csharp
Contains()
Substring()
Replace()
Split()
Trim()
ToUpper()
ToLower()
```

## StringBuilder

```csharp
StringBuilder
```

## String Interpolation

```csharp
$"Hello {name}"
```

---

# 12. Exception Handling

## try catch

```csharp
try
{
}
catch(Exception ex)
{
}
```

## finally

## throw

## Custom Exceptions

---

# 13. File Handling

## File Class

## StreamReader

## StreamWriter

## Directory Class

## Path Class

## Serialization

- JSON Serialization
- XML Serialization

---

# 14. Delegates and Events

## Delegates

```csharp
delegate
```

## Action

## Func

## Predicate

## Events

## EventHandler

## Lambda Expressions

```csharp
x => x * 2
```

---

# 15. LINQ

## LINQ Basics

## Where

## Select

## OrderBy

## GroupBy

## Any

## All

## First / FirstOrDefault

## LINQ Query Syntax

## LINQ Method Syntax

---

# 16. Generics

## Generic Classes

## Generic Methods

## Generic Constraints

---

# 17. Async Programming

## async and await

```csharp
async
await
```

## Task

## Task<T>

## Parallel Programming

## Threading Basics

## CancellationToken

---

# 18. Memory Management

## Stack vs Heap

## Garbage Collection (GC)

## IDisposable

## using Statement

## Boxing and Unboxing

```csharp
object obj = 10; // boxing
int x = (int)obj; // unboxing
```

---

# 19. Advanced C# Concepts

## Reflection

## Attributes

## Indexers

## Extension Methods

## Anonymous Types

## Nullable Reference Types

## Pattern Matching

## Tuples

## Records

## Span<T>

## Dependency Injection

## Expression Trees

---

# 20. .NET Related Topics

## .NET Framework

- Windows only
- Legacy applications

## .NET Core

- Cross-platform
- Modern development

## .NET 5+

- Unified platform

## Latest .NET Versions

- .NET 8 (LTS)
- .NET 9

## ASP.NET Core

- Web APIs
- MVC
- Razor Pages
- Blazor

## Entity Framework Core

- ORM
- Migrations
- LINQ Queries

## Minimal APIs

## Middleware

## Dependency Injection in ASP.NET Core

---

# 21. Desktop Development

## Windows Forms

## WPF

## MAUI

---

# 22. Database Concepts

## SQL Basics

## CRUD Operations

## Relationships

## Stored Procedures

## Indexing

## Transactions

## Entity Framework Core

## Dapper

---

# 23. API Development

## REST APIs

## HTTP Methods

```text
GET
POST
PUT
DELETE
PATCH
```

## Status Codes

## JSON Handling

## Authentication

- JWT
- OAuth
- Cookies

## Swagger

---

# 24. Testing

## Unit Testing

## xUnit

## NUnit

## Moq

## Integration Testing

---

# 25. Design Patterns

## Singleton

## Repository Pattern

## Factory Pattern

## Dependency Injection

## CQRS

## Mediator Pattern

---

# 26. Security Concepts

## Authentication

## Authorization

## Hashing

## Encryption

## Secure Coding Practices

## HTTPS

## CORS

---

# 27. DevOps and Deployment

## Git and GitHub

## CI/CD

## Docker

## Kubernetes Basics

## Azure Basics

## AWS Basics

## IIS Hosting

## Nginx Reverse Proxy

---

# 28. Performance Optimization

## Caching

## Memory Optimization

## Async Optimization

## Database Optimization

## Profiling

---

# 29. Useful Tools

## Postman

## Swagger

## SQL Server Management Studio

## Visual Studio

## Rider

## dotnet CLI

---

# 30. Recommended Learning Order

1. Basics of C#
2. Variables and Data Types
3. OOP Concepts
4. Collections and LINQ
5. Exception Handling
6. Async Programming
7. ASP.NET Core
8. Database Integration
9. APIs
10. Authentication
11. Testing
12. Docker and Deployment
13. Design Patterns
14. Cloud and DevOps

---

# 31. Common Interview Topics

## Beginner

- Data Types
- Value vs Reference Types
- Arrays
- OOP Basics
- Loops
- Methods

## Intermediate

- LINQ
- Delegates
- Events
- Async Await
- Exception Handling
- Collections

## Advanced

- Dependency Injection
- Middleware
- Entity Framework
- Garbage Collection
- Design Patterns
- Multithreading

---

# 32. Important Keywords to Learn

```text
class
struct
interface
abstract
virtual
override
sealed
readonly
const
static
async
await
var
dynamic
base
this
new
using
namespace
record
partial
```

---

# 33. Suggested Practice Projects

## Beginner Projects

- Calculator
- ToDo App
- Student Management System
- Library Management System

## Intermediate Projects

- REST API
- Authentication System
- E-commerce Backend
- Chat Application

## Advanced Projects

- Microservices
- Real-time Application with SignalR
- Distributed Systems
- Cloud-based Application

---

# 34. Important Concepts for Backend Development

## ASP.NET Core

## Middleware Pipeline

## Authentication and Authorization

## Dependency Injection

## Entity Framework Core

## Repository Pattern

## Logging

## Background Services

## Caching

## Message Queues

- RabbitMQ
- Kafka

## Microservices

---

# 35. Additional Topics Worth Exploring

## SignalR

## GraphQL

## WebSockets

## gRPC

## Clean Architecture

## Domain Driven Design (DDD)

## Event Driven Architecture

## Microservices Architecture

## Azure Services

## AWS Services

---

# Key Focus Areas

- Strong C# fundamentals
- OOP concepts
- Collections and LINQ
- ASP.NET Core
- Databases and APIs
- Async programming
- Design patterns
- Deployment and DevOps
