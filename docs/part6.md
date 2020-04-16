---
title: "Part 6 - UML Diagram tools"
permalink: /part6/
nav_order: 8
published: true
---

## Part 6

*"The Unified Modeling Language (UML) is a general-purpose, developmental, modeling language in the field of software engineering that is intended to provide a standard way to visualize the design of a system."* [**(Wikipedia)**](https://en.wikipedia.org/wiki/Unified_Modeling_Language)

UML is the most wide-spread way to create diagrams for documentation. There are plenty of different diagram types to choose from, but we will concentrate on a couple: class diagram and sequence diagram, and the tools for making them. You can find more about [**class diagrams here**](https://en.wikipedia.org/wiki/Class_diagram) and [**sequence diagrams here**](https://en.wikipedia.org/wiki/Sequence_diagram).

One very popular tool for drawing diagrams is [**Yuml.me**](https://yuml.me). You can draw any diagrams, but class diagrams are by far the most popular use for the tool. The strength of this tool is in the way the diagrams are represented: as code. When usually diagram tools are focused on drawing the tool, with Yuml.me you can write your diagram as code. The downside is, that with large diagrams, you have to do quite much writing.

Another tool, meant for sequence diagrams, is [**Sequencediagram.org**](https://sequencediagram.org/). The working functionality is similar to that of the Yuml.me, so you can write your diagram as code, and the tool will draw your diagram based on that.

NOTICE! The notation for both of these tools are different, and tool specific. 

Third tool, which is more versatile but has bit of a learning curve, is [**Draw.io**](https://draw.io). With this tool, you can create any charts. This time the charts are not done by code, but by placing elements on a grid or canvas, or if you feel adventurous, drawing freehand.

Finally, [**LucidChart**](https://lucidchart.com) is a commercial tool for drawing all UML charts. You can also have a free trial for the software. It is a very versatile tool, and quite used in the industry. 

NOTICE! Refreshing the web page on any of these tools might lose your work. Remember to save your code or picture after you are done.

### By yourself or as a group

* Read the material behind the three links:
  * [**UML**](https://en.wikipedia.org/wiki/Unified_Modeling_Language)
  * [**Class diagrams**](https://en.wikipedia.org/wiki/Class_diagram)
  * [**sequence diagrams**](https://en.wikipedia.org/wiki/Sequence_diagram)

* You should also watch this video: [**How to make a UML Sequence Diagram**](https://www.youtube.com/watch?v=pCK6prSq8aw)

* Familiarize yourself (or yourselves) with the tools above. **If you are already familiar with other tools for this, you can use those**. Just fiddle around, no need to do anything special (yet).


Deadline for these is **21.4.2020 at 23:59**.  

### As a group


* The customer really liked your software so far. They want you to extend the project. After a discussion with the customer, they give you the requirements:

*We need an abstract class **Animal**, which all the animals inherit. The Animal must have a method **MakeSound**. The previous method **TalkToOwner** can stay for tame animals. We want to divide the animals into subcategories, into tame and wild animals. Make these into **interfaces**, **ITame** and **IWild**, respectively. The ITame interface should have property **name** and a method **string ComeHere()**, which returns "\<name\> came to the owner.", where \<name\> is the name of the animal. The IWild animals should not have a name, but a method **string Hunt**, which returns "\<Type\> hunts", where \<Type\> is the type (or class) of the animal. Also add the wild animals **Bear**, **Wolf** and **Tiger**. The folder structure should be something in the line of:*

```console
.
├── README.md
├── assets
│    └── class_diagram_with_connections.png
│ 
├── src
│    └── Fauna
│         ├── Animals
│         │       ├── Animal.cs
│         │       ├── Wild
│         │       │    ├── IWild.cs
│         │       │    ├── Wolf.cs
│         │       │    ├── Bear.cs
│         │       │    └── Tiger.cs
│         │       └── Tame
│         │            ├── ITame.cs
│         │            ├── Cat.cs
│         │            ├── Bird.cs
│         │            └── Dog.cs
│         ├── Fauna.csproj
│         └── Program.cs
└── test
    └── FaunaTests
          ├── FaunaTest.cs
          └──  FaunaTests.csproj
```

* **Update your program with these instructions**, using the proper ways of Kanban.
* If in your Trello board something is done, **do not touch it**.
* All new tasks require new cards. That's how the board works.
* Everyone should contribute, doing at least one task (one new. animal, interface, etc). Try to divide the job evenly.
* When you take a task from the board, add yourself to the card as a Member.
* Create **class diagrams**, with their connections, to all your classes and interfaces, and save it in the **assets** folder, as shown in the structure. You should end up with one picture, where all the animals implement one of the interfaces, and all the animals inherit the abstract class. Program.cs does not need a diagram.

Deadline for the group task is **28.4.2020 at 23:59**.  