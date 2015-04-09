class: center, middle

# Scala Days 2015 Recap
### Steven Gangstead
### slides https://gangstead.github.io/scaladays-2015-recap
@Gangstead
.footnote[.round[![:scale 20%](slides/credera.jpg)]]
---

# Scala Days 2015

- Match 16-19, San Francisco

---

# Keynotes

- Martin Oderksy : **_Scala - where it came from, where it's going_**
- Danese Cooper : **_Why Open Languages Win_**
- Dianne Marsh : **_Technical Leadership from wherever you are_**

---

# Martin Oderksy : **_Scala - where it came from, where it's going_**
## Where it came from
- He created a language called `Pizza` in the mid 90's
 - Super set of Java with generics, first-class functions, case classes and pattern matching (sound familiar?)
 - Eventually led to generics in Java 1.5
- With EPFL he created another FP language `Funnel` (not on JVM)
- 2002 Started working on Scala at EPFL
.footnote[Slides: http://www.slideshare.net/Odersky/scala-days-san-francisco-45917092]
---

# Martin Oderksy : **_Scala - where it came from, where it's going_**
What makes Scala Scala?
- functional
- obect-oriented / modular
- statically typed
- strict
- closest predecessor: OCaml
 - Differences: OCaml separates object and module system, Scala unifies them
 - OCaml uses Hindley/Milner, Scala subtyping + local type inference.

---

# Martin Oderksy : **_Scala - where it came from, where it's going_**

- 1st Invariant: A Scalable Language
 - Instead of providing lots of features in the language, have the right abstractions so that they can be provided in libraries
- 2nd Invariant: It's all about the types
 - Scala's core is its type system
 - Scala's initial main goal is to make the type system good enough for people who would otherwise choose a dynamic language (focus on flexibility over safety)
 - The goal is for Scala to catch up in terms of Type Safety with other typed languages
---

# Martin Oderksy : **_Scala - where it came from, where it's going_**
## The Present

- Emergent Ecosystem
- Now targets JS (Scala.JS no longer experimental)
- Tooling getting better
 - faster incremental compiles in sbt and ides
 - Better support for Eclipse, IntelliJ (JetBrains was a sponsor), Ensime (emacs plugin)
- Coursera class has 400k "inscriptions", Success rate ~10% (higher than industry average)
---

# Martin Oderksy : **_Scala - where it came from, where it's going_**
## The Future

- Emergence of a "reactive" platform
 - Core libraries + Specifications like Futures, Reactive Streams, Spores
 - Analogous to Java EE (*audience groans*)

---

# Martin Oderksy : **_Scala - where it came from, where it's going_**

- The JDK is the core of the Java platform, relies on class files as the intermediary between Java code and native code.
- Currently Scala piggy backs off of this (class files + scala signatures)
 - Already having binary compatibility problems between Scala releases, what about future JDK increments, new targets like JS?
- New proposal `TASTY`
 - Serialized Typed Abstract Syntax Trees

---

# Martin Oderksy : **_Scala - where it came from, where it's going_**
![:scale 60%](slides/TASTY.png)

---

# Martin Oderksy : **_Scala - where it came from, where it's going_**
## TASTY

- 25% class file size
- code analysis, refactoring
- Automated remapping = solve binary compatibility
- Just a spec at this point

---

# Martin Oderksy : **_Scala - where it came from, where it's going_**
Other things
- DOT: Dependent Object Types
 - New foundation for Scala's type system (?)
 - Cleaned up version of Scala, no working implementation yet
- Exploring:
 - Implicits that compose (slide 42)
 - Better treatment of effects (mutation, IO, exceptions...) with something better than Monads, like implicits to model effects

---

# Martin Oderksy : **_Scala - where it came from, where it's going_**
Conclusion:
- Scala established FP for the mainstream
- showed that a fusion of OOP and FP is both possible and useful
- promoted the adoption of strong static typing

Aims:
- Make platform more powerful
- make the language simpler
- work on foundations to get to the essence of Scala

---


# Akka-http

```scala
really cool akka-http code example
```
---

# The End
## My Notes
### https://gist.github.com/gangstead/e0955e77864e318bc61e

- Shameless Plug for NodeSchool
 - Next meetup 4/22
 - Express.js web framework
 - http://www.meetup.com/Nodeschool-Dallas/events/219510528/
