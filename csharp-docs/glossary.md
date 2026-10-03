# Glossary

Short, beginner-friendly definitions of common C# and .NET terms.

---

## A

**Argument**  
The actual value you pass to a method when you call it. In `Console.WriteLine("Hello")`, `"Hello"` is the argument.

**API (Application Programming Interface)**  
The set of classes, methods, properties, and types that a library or framework exposes for you to use.

**Assembly**  
A compiled unit of code (a `.dll` or `.exe` file) that contains types and resources. Your project compiles into an assembly.

**Async / Asynchronous**  
Code that can wait for something (like a file download or database query) without blocking the current thread. See `async/overview.md`.

---

## B

**Base Class**  
The class that another class inherits from. In `class Dog : Animal`, `Animal` is the base class.

**Boolean / bool**  
A type that can only be `true` or `false`.

**Breakpoint**  
A marker in your code that tells the debugger to pause execution so you can inspect variables.

**Build**  
The process of compiling your source code into an executable program or library.

---

## C

**Call Stack**  
The list of method calls that led to the current point in execution. The debugger shows this when paused.

**Class**  
A blueprint for creating objects. Defines fields, properties, methods, and events.

**Collection**  
A type that stores multiple values. Examples: `List<T>`, `Dictionary<TKey,TValue>`, `Array`.

**Compiler**  
The program (`csc` or Roslyn) that translates your C# source code into IL (Intermediate Language).

**Console Application**  
A program that runs in a text-based terminal window. The default project type for beginners.

**Constructor**  
A special method that runs when you create a new instance of a class. Same name as the class, no return type.

---

## D

**Delegate**  
A type that represents a reference to a method. Used for callbacks and events.

**Derived Class**  
A class that inherits from a base class. In `class Dog : Animal`, `Dog` is the derived class.

**Dispose / IDisposable**  
A pattern for cleaning up unmanaged resources (files, database connections, etc.) deterministically. See `utilities/disposable.md`.

---

## E

**Enum (Enumeration)**  
A value type that defines a set of named constants. Example: `enum Day { Mon, Tue, Wed }`.

**Exception**  
An error condition that disrupts normal program flow. Caught with `try`/`catch`. See `exceptions/overview.md`.

**Expression**  
A piece of code that produces a value. `5 + 3`, `"hello"`, `x > 0` are all expressions.

**Extension Method**  
A static method that can be called as if it were an instance method on another type. LINQ methods like `Where()` are extension methods.

---

## F

**Field**  
A variable declared directly inside a class or struct. Holds state for each instance.

**Framework**  
The set of libraries and runtime that your code runs on. ".NET" is the framework; ".NET 8" is a version.

---

## G

**Generic**  
A class or method that works with a type parameter (`<T>`). Example: `List<T>` works with `List<int>`, `List<string>`, etc. See `generics.md`.

**Garbage Collector (GC)**  
The automatic memory manager that reclaims memory from objects no longer in use.

---

## H

**Heap**  
Memory region where reference-type objects (classes) are allocated. Managed by the GC.

---

## I

**IL (Intermediate Language)**  
The low-level, platform-agnostic code that C# compiles to. The runtime (CLR) executes IL.

**Immutable**  
Cannot be changed after creation. `string` is immutable—every "modification" creates a new string.

**Inheritance**  
A mechanism where a derived class reuses and extends the behavior of a base class.

**Interface**  
A contract that defines what methods/properties a class must have, without implementation.

**Instance**  
A specific object created from a class blueprint. `new Dog()` creates an instance of `Dog`.

**Iteration**  
Going through a collection one item at a time (e.g., with `foreach`).

---

## K

**Keyword**  
A reserved word with special meaning to the compiler (e.g., `class`, `if`, `while`, `return`).

---

## L

**Lambda Expression**  
A concise way to write an anonymous function. `x => x * 2` is a lambda that doubles its input.

**Local Variable**  
A variable declared inside a method. Only exists while that method runs.

---

## M

**Method**  
A named block of code that performs an action. Can take parameters and return a value.

**Mutable**  
Can be changed after creation. `List<T>` is mutable—you can add/remove items.

**Namespace**  
A logical grouping of types to avoid name collisions. `System.Collections.Generic` contains `List<T>`.

**Null**  
The absence of a value. Reference types can be null; value types cannot (unless nullable: `int?`).

**Nullable Type**  
A value type that can also hold `null`. Written as `int?` (shorthand for `Nullable<int>`).

---

## O

**Object**  
An instance of a class. Sometimes used to mean `System.Object`, the base type of all types.

**Overload**  
Multiple methods with the same name but different parameters.

**Override**  
A derived class providing a new implementation for a virtual/abstract member from the base class.

---

## P

**Parameter**  
A variable in a method definition that receives an argument. In `void Greet(string name)`, `name` is the parameter.

**Polymorphism**  
The ability to treat derived classes as their base class, with the correct method running at runtime.

**Primitive Type**  
Built-in simple types like `int`, `double`, `bool`, `char`.

**Project**  
A `.csproj` file and its source files. Compiles into one assembly.

**Property**  
A member that looks like a field but has getter/setter logic. `public string Name { get; set; }`

---

## R

**Reference Type**  
A type that stores a reference to data on the heap. Classes, arrays, delegates, interfaces. See `value-vs-reference-types.md`.

**Runtime**  
The environment that executes your compiled code (.NET Runtime / CLR).

---

## S

**Scope**  
The region of code where a variable is visible. Defined by `{ }` braces.

**Serialization**  
Converting an object into a format that can be stored or transmitted (JSON, XML, binary).

**Solution (.sln)**  
A container for one or more related projects.

**Stack**  
Memory region for value types and method call frames. Fast, automatically managed.

**Statement**  
A complete instruction ending with `;`. `int x = 5;` is a statement.

**Static**  
Belongs to the type itself, not to an instance. `Console.WriteLine` is static.

**String**  
An immutable sequence of characters. `string` is an alias for `System.String`.

**Struct**  
A value type that can have fields, properties, methods. Copied by value. See `fundamentals/structs.md`.

---

## T

**Thread**  
A path of execution within a process. Multiple threads can run simultaneously.

**Type**  
A classification that defines what values a variable can hold and what operations are valid.

**Tuple**  
A lightweight group of values. `(string Name, int Age)` is a tuple.

---

## V

**Value Type**  
A type that stores its data directly (on the stack or inline). `int`, `bool`, `struct`, `enum`. See `value-vs-reference-types.md`.

**Variable**  
A named storage location with a type. `int age = 18;`

**Virtual**  
A method/property that can be overridden in a derived class.

---

## Other

**`var`**  
Implicit typing—the compiler infers the type from the initialization expression. `var x = 5;` makes `x` an `int`.

**`.NET SDK`**  
The toolchain (compiler, CLI, libraries) you install to build .NET apps.

**`dotnet` CLI**  
Command-line interface for creating, building, running, and publishing .NET projects.

**`NuGet`**  
The package manager for .NET libraries.