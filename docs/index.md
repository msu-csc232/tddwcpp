# Welcome to CSC232!

## CSC232 - Data Structures

CSC232 is a continuation of CSC 131. Topics will include: algorithm design; complexity analysis; abstract data types and encapsulation; basic data structures and their application, including stacks, queues, linked lists and binary trees; dynamic memory allocation; recursion; sorting and searching; debugging techniques.

_**Prerequisite**: "C" or better in CSC 131; and MTH 261 or MTH 314 or MTH 315 or concurrent enrollment._

## Topics

* Review C++ Fundamentals
* Collections
* Sorting Algorithms
* Lists and Sorted Lists
* Stacks
* Queues and Priority Queues
* Trees

## Approach

* Hands-on, Test-Driven Development
* Continuous Development of the Analysis of Algorithms

## Admonitions

!!! info inline end

    Lorem ipsum dolor sit amet, consectetur
    adipiscing elit.

This site uses a number of _admonitions_ to highlight different points in different ways. For example, to the right of this paragraph, we see an inline note. Such an inline note may be used to highlight an ancillary point to the current topic. As you can see, the note floats to the right. Sometimes this will float on the left (by removing the `end` qualifier to the `inline` admonition).

???+ note

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

???+ abstract "Abstract, Summary, or TLDR"

    abstract, summary, tldr

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

???+ info "Info, or TODO"

    info, todo

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

???+ tip "Tip, Hint, or Important"

    tip, hint, important

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

???+ success "Success, Check, or Done"

    success, check, done
    
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

???+ question "Question, Help, or FAQ"

    question, help, faq
    
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

???+ warning "Warning, Caution, or Attention"

    warning, caution, attention
    
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

???+ failure "Failure, Fail, or Missing"

    failure, fail, missing
    
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

???+ danger "Danger, or Error"

    danger, error
    
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

???+ bug

    bug
    
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

???+ example "Example"

    example
    
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

???+ quote "Quote, or Cite"

    quote, cite
    
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

See [https://squidfunk.github.io/mkdocs-material/reference/admonitions/#usage](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#usage)

## Diagrams

### Flowcharts

Flowcharts are diagrams that represent workflows or processes. The steps are rendered as nodes of various kinds and are connected by edges, describing the necessary order of steps:

``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```

### Sequence Diagrams

Sequence diagrams describe a specific scenario as sequential interactions between multiple objects or actors, including the messages that are exchanged between those actors:

``` mermaid
sequenceDiagram
  Alice->>John: Hello John, how are you?
  loop Healthcheck
      John->>John: Fight against hypochondria
  end
  Note right of John: Rational thoughts!
  John-->>Alice: Great!
  John->>Bob: How about you?
  Bob-->>John: Jolly good!
```

### State Diagrams

State diagrams are a great tool to describe the behavior of a system, decomposing it into a finite number of states, and transitions between those states:

``` mermaid
stateDiagram-v2
  state fork_state <<fork>>
    [*] --> fork_state
    fork_state --> State2
    fork_state --> State3

    state join_state <<join>>
    State2 --> join_state
    State3 --> join_state
    join_state --> State4
    State4 --> [*]
```

### Class Diagrams

Class diagrams are central to object oriented programing, describing the structure of a system by modelling entities as classes and relationships between them:

``` mermaid
classDiagram
  Person <|-- Student
  Person <|-- Professor
  Person : +String name
  Person : +String phoneNumber
  Person : +String emailAddress
  Person: +purchaseParkingPass()
  Address "1" <-- "0..1" Person:lives at
  class Student{
    +int studentNumber
    +int averageMark
    +isEligibleToEnrol()
    +getSeminarsTaken()
  }
  class Professor{
    +int salary
  }
  class Address{
    +String street
    +String city
    +String state
    +int postalCode
    +String country
    -validate()
    +outputAsLabel()  
  }
```
