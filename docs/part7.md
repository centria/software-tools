---
title: "Part 7 - Final project"
permalink: /part7/
nav_order: 9
published: true
---

## Part 7

### This is the Final Project of the course.

The deadline for this final project is **17.5.2020 at 23:59:59**. By then, 
* all the commits should be in GitHub
* Trello should be up to date
* Documentation should be up to par

As usual, the customer is satisfied to your work, but demands changes, as well as new features to your program.

*"I want to have a **TextInterface**, where I can try out all the animals! The program should be able to list all the animals that are have been created. After this, it could ask for which animal to see, and then list all the methods of an animal. Then I want to be able to use those methods, and exit the program nicely with 'quit' or something similar."*

The customer continues:

*"I want the animals to be able to **Eat()**! When a tame animal eats, they gain 1kg weight. Oh, they don't have weight? All animals should have property **weight**. Better make that abstract, then? Where was I. Yes, tame animals gain 1kg when they eat. Wild animals should use the eat method inside their **Hunt** method, but they are not always lucky. They should succeed with a 60% chance to eat while hunting."*

*"... And it would be nice, if pets could also be given names in the program."*

An example for tame animals follows. Your execution does not have to be 100% same, this is just a concept:

```console
What do you want to do? [list, quit]
> list
List of animals:
Wolf
Tiger
Bear
Cat
Dog
Bird
Which animal do you want to see?
> Cat

What do you want to do? [Eat, TalkToOwner, MakeSound, ComeHere, GiveName, back, quit]
> ComeHere

Cat came to the owner.
What do you want to do? [Eat, TalkToOwner, MakeSound, ComeHere, GiveName, back, quit]
> GiveName

Give a name:
> Garfield

What do you want to do? [Eat, TalkToOwner, MakeSound, ComeHere, GiveName, back, quit]
> Eat

Garfield gained 1 kg, and weighs now 1 kg.
What do you want to do? [list, quit]
> quit

```

For wild animals, something like this could happen. This could be another way of doing the TextInterface, the implementation is up to you:

```console
What do you want to do?
0 - quit
1 - list
> 1
List of animals:
0 - quit
1 - back
2 - Wolf
3 - Tiger
4 - Bear
5 - Cat
6 - Dog
7 - Bird
> 4
What do you want to do? 
0 - quit
1 - back
2 - MakeSound
3 - Hunt
> 3
Bear finds food, gains 1 kg and weighs now 1 kg.
What do you want to do? 
0 - quit
1 - back
2 - MakeSound
3 - Hunt
> 3
Bear does not find food and weighs 1 kg.
What do you want to do? 
0 - quit
1 - back
2 - MakeSound
3 - Hunt
> 3
Bear finds food, gains 1 kg and weighs now 2 kg.
What do you want to do? 
0 - quit
1 - back
2 - MakeSound
3 - Hunt
> 2
What do you want to do?
0 - quit
1 - list
> 0
```

*"Oh, I also want to have **sequence diagrams** for those examples.*

*If you haven't already, I also want tests for all the methods. You don't have to test the TextInterface, but you can if you want to.*

*Ah, I almost forgot. The project should have a proper README.md in the root folder, which describes the project."*


* **Update your program with these instructions**, using the proper ways of Kanban.
  * TextInterface
  * Tests
  * New and updated methods
  * etc, etc, etc...
* If in your Trello board something is done, **do not touch it**.
* All new tasks require new cards. That's how the board works.
  * TextInterface
  * Tests
  * Diagrams
  * Documentation
  * etc, etc, etc...
* Everyone should contribute, doing at least one task. Try to divide the job as evenly as possible.
* When you take a task from the board, add yourself to the card as a Member. Multiple people can work on a single task, but it is adviced to split tasks as small as possible.
* Keep the project structure clean.
* Create **sequence diagrams** following the two examples given above, or something at least as complicated, where user gives some inputs and then quits. Make the diagram following your program logic and UI. Save it to the same location as the class diagram from before. You can use the [**Sequencediagram.org**](https://sequencediagram.org/) introduced in the previous part, or any other tool you like.
* In the README.md file, you should have at least:
  * A topic / name for your project.
  * Link to the Trello board, or a picture of the final status.
  * Short description of the project (few sentences).
  * Class diagram and short descrition for it.
  * Sequence diagram with short description.
  * Project's folder structure (you can use the **tree** command from unix, for example)
* Use proper [**Markdown notation**](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) in your documentation, i.e. have topics and subtopics as different level topics, embed the pictures in the document (and not just as links) etc.
