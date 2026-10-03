# C#/.NET Offline Beginner Handbook

Welcome to your personal offline C# reference! This handbook is designed for beginners learning C# with **VS Code**, **C# Dev Kit**, and the **.NET SDK** on Windows.

## What This Handbook Is

- A practical, beginner-friendly reference you can keep locally
- Focused on the language features, classes, methods, and APIs you'll actually use while learning
- Organized so you can find answers quickly when you're offline
- Written in plain English with runnable examples

## What This Handbook Is Not

- A complete copy of Microsoft Learn or the .NET API reference
- An advanced language specification
- A replacement for official documentation when you need deep technical details

## Who This Is For

You're learning C# fundamentals and want a searchable, offline companion that answers questions like:

- "How do I print something?"
- "How do I convert a string to an integer?"
- "Should I use an array or a List?"
- "How do I read a text file?"
- "What does `async` actually do?"
- "How do I catch an error?"
- "What namespace do I need?"

## Folder Structure

```
csharp-docs/
├── README.md                    # This file - start here
├── glossary.md                  # Beginner definitions of common terms
├── cheatsheet.md                # Quick syntax reference
├── common-errors.md             # Compiler/runtime error explanations
├── project-basics.md            # .NET CLI commands, project structure
├── debugging.md                 # VS Code debugging guide
├── naming-conventions.md        # C# naming standards
├── type-system.md               # Value types vs reference types overview
├── value-vs-reference-types.md  # Deep dive on value/reference semantics
├── generics.md                  # Understanding <T> syntax
│
├── fundamentals/                # Core language concepts
│   ├── variables.md
│   ├── data-types.md
│   ├── operators.md
│   ├── conditions.md
│   ├── loops.md
│   ├── methods.md
│   ├── parameters.md
│   ├── scope.md
│   ├── classes.md
│   ├── objects.md
│   ├── constructors.md
│   ├── properties.md
│   ├── fields.md
│   ├── access-modifiers.md
│   ├── static.md
│   ├── inheritance.md
│   ├── interfaces.md
│   ├── abstract-classes.md
│   ├── structs.md
│   ├── enums.md
│   ├── records.md
│   ├── tuples.md
│   ├── pattern-matching.md
│   └── switch-expressions.md
│
├── system/                      # Core System namespace APIs
│   ├── console.md
│   ├── math.md
│   ├── convert.md
│   ├── string.md
│   ├── char.md
│   ├── datetime.md
│   ├── timespan.md
│   ├── datetimeoffset.md
│   ├── random.md
│   ├── guid.md
│   ├── environment.md
│   ├── uri.md
│   └── version.md
│
├── numbers/                     # Numeric parsing, formatting, types
│   ├── parsing.md
│   ├── numeric-types.md
│   ├── formatting.md
│   └── rounding.md
│
├── collections/                 # Data structures
│   ├── overview.md
│   ├── array.md
│   ├── list.md
│   ├── dictionary.md
│   ├── hashset.md
│   ├── queue.md
│   ├── stack.md
│   ├── linkedlist.md
│   ├── priorityqueue.md
│   └── enumerable.md
│
├── linq/                        # Language Integrated Query
│   ├── overview.md
│   ├── filtering.md
│   ├── projection.md
│   ├── sorting.md
│   ├── searching.md
│   ├── checking.md
│   ├── aggregation.md
│   ├── grouping.md
│   ├── set-operations.md
│   ├── partitioning.md
│   └── conversion.md
│
├── files/                       # File system operations
│   ├── overview.md
│   ├── file.md
│   ├── directory.md
│   ├── path.md
│   ├── fileinfo.md
│   ├── directoryinfo.md
│   ├── streamreader.md
│   ├── streamwriter.md
│   └── streams.md
│
├── text/                        # Advanced text processing
│   ├── stringbuilder.md
│   ├── regex.md
│   ├── encoding.md
│   └── text-formatting.md
│
├── json/                        # JSON serialization
│   ├── overview.md
│   ├── jsonserializer.md
│   ├── serializer-options.md
│   └── jsondocument.md
│
├── networking/                  # HTTP and networking
│   ├── overview.md
│   ├── httpclient.md
│   ├── httpresponsemessage.md
│   └── http-basics.md
│
├── async/                       # Asynchronous programming
│   ├── overview.md
│   ├── task.md
│   ├── async-await.md
│   ├── task-delay.md
│   ├── task-whenall.md
│   └── cancellationtoken.md
│
├── exceptions/                  # Error handling
│   ├── overview.md
│   ├── try-catch-finally.md
│   ├── throwing-exceptions.md
│   └── common-exceptions.md
│
├── diagnostics/                 # Performance and debugging tools
│   ├── stopwatch.md
│   ├── debug.md
│   └── tracing-basics.md
│
└── utilities/                   # Helper APIs and patterns
    ├── nullable.md
    ├── enum-utilities.md
    ├── object-methods.md
    ├── comparer.md
    ├── equality.md
    ├── disposable.md
    ├── using-statement.md
    ├── console-input-validation.md
    └── useful-methods.md
```

## How to Use This in VS Code

1. **Open the folder**: File → Open Folder → select `csharp-docs`
2. **Search across files**: Press `Ctrl+Shift+F` to search all Markdown files at once
3. **Navigate with links**: Ctrl+Click any relative link to jump to that file
4. **Side-by-side editing**: Right-click a tab → "Split Right" to view docs while coding

## Code Examples in This Handbook

You'll see two styles of C# code examples:

### Top-Level Statements (Modern, .NET 6+)

```csharp
using System;

Console.WriteLine("Hello, World!");
```

This is the default for new console projects (`dotnet new console`). No `class Program` or `Main` method needed.

### Traditional Style (Classic, All Versions)

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Hello, World!");
    }
}
```

Both styles compile to the same thing. The handbook uses **both** so you recognize either in real code. When an example uses top-level statements, it works directly in a modern console project. When you see `class Program`, you can paste it into any C# file.

## What Should I Learn First?

If you're just starting, follow this rough order. You don't need to master each topic completely before moving on—just get comfortable with the basics.

| Order | Topic | Files to Read |
|-------|-------|---------------|
| 1 | Variables & Data Types | `fundamentals/variables.md`, `fundamentals/data-types.md` |
| 2 | Operators | `fundamentals/operators.md` |
| 3 | Conditions (`if`/`else`) | `fundamentals/conditions.md` |
| 4 | Loops (`for`/`foreach`/`while`) | `fundamentals/loops.md` |
| 5 | Methods | `fundamentals/methods.md`, `fundamentals/parameters.md` |
| 6 | Arrays & Lists | `collections/array.md`, `collections/list.md` |
| 7 | Classes & Objects | `fundamentals/classes.md`, `fundamentals/objects.md` |
| 8 | Dictionaries | `collections/dictionary.md` |
| 9 | Exceptions | `exceptions/try-catch-finally.md` |
| 10 | LINQ Basics | `linq/overview.md`, `linq/filtering.md`, `linq/projection.md` |
| 11 | File I/O | `files/file.md`, `files/directory.md`, `files/path.md` |
| 12 | JSON | `json/overview.md`, `json/jsonserializer.md` |
| 13 | Async/Await | `async/async-await.md`, `async/task.md` |
| 14 | HTTP Requests | `networking/httpclient.md` |

## Quick Task → Documentation Table

| I want to... | Read |
|---|---|
| Print something | `system/console.md` |
| Read keyboard input | `system/console.md` |
| Convert text to a number | `numbers/parsing.md` |
| Store several values | `collections/list.md` |
| Store fixed-size values | `collections/array.md` |
| Store key/value pairs | `collections/dictionary.md` |
| Store unique values | `collections/hashset.md` |
| Process items in arrival order | `collections/queue.md` |
| Process newest items first | `collections/stack.md` |
| Filter a collection | `linq/filtering.md` |
| Transform collection items | `linq/projection.md` |
| Sort data | `linq/sorting.md` |
| Find an item | `linq/searching.md` |
| Calculate a sum or average | `linq/aggregation.md` |
| Work with dates | `system/datetime.md` |
| Work with durations | `system/timespan.md` |
| Generate random numbers | `system/random.md` |
| Generate a unique ID | `system/guid.md` |
| Manipulate text | `system/string.md` |
| Build large strings | `text/stringbuilder.md` |
| Search using patterns | `text/regex.md` |
| Read or write files | `files/file.md` |
| Work with folders | `files/directory.md` |
| Build file paths | `files/path.md` |
| Serialize JSON | `json/jsonserializer.md` |
| Make an HTTP request | `networking/httpclient.md` |
| Run asynchronous operations | `async/async-await.md` |
| Wait without blocking | `async/task-delay.md` |
| Run async operations together | `async/task-whenall.md` |
| Handle errors | `exceptions/try-catch-finally.md` |
| Handle null values | `utilities/nullable.md` |
| Measure execution time | `diagnostics/stopwatch.md` |
| Debug my program | `debugging.md` |
| Understand a compiler error | `common-errors.md` |

## How Relative Links Work

All links in this handbook use **relative paths**. For example, from `fundamentals/variables.md`, a link to `../system/console.md` means "go up one folder, then into `system`, then open `console.md`."

If you move files around, links may break. Keep the folder structure intact.

## Conventions Used

- **`code`** — inline code, keywords, method names
- **`Type`** — class, struct, interface names
- **`method()`** — methods (parentheses indicate it's callable)
- **`Property`** — properties (no parentheses)
- **⚠️ Warning** — common mistakes to avoid
- **💡 Tip** — helpful shortcuts or best practices
- **📝 Note** — extra context worth knowing
- **✅ Essential** — core concepts every beginner should learn
- **🔧 Useful** — common in real projects
- **📚 Learn Later** — worth recognizing but not essential now

---

**Start reading**: [What should I learn first?](#what-should-i-learn-first) or jump to [glossary.md](glossary.md) if you encounter an unfamiliar term.