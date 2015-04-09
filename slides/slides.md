class: center, middle

# Scala Days 2015 Recap
### Steven Gangstead
### slides https://gangstead.github.io/scaladays-2015-recap
@Gangstead
.footnote[.round[![:scale 20%](slides/credera.jpg)]]
---

# Scala Days 2015

- Match 16-19, San Francisco
- Keynotes - detailed
- Sessions I attended - 10,000 ft view
- Trivia - fabulous prizes
---
class: center
# View from Fort Mason center
![:scale 60%](slides/ggbridge.jpg)
---
class: center, middle
# Keynotes

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
class: center
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
### Other things
- DOT: Dependent Object Types
 - New foundation for Scala's type system (?)
 - Cleaned up version of Scala, no working implementation yet
- Exploring:
 - Implicits that compose (slide 42)
 - Better treatment of effects (mutation, IO, exceptions...) with something better than Monads, like implicits to model effects

---

# Martin Oderksy : **_Scala - where it came from, where it's going_**
### Conclusion:
- Scala established FP for the mainstream
- showed that a fusion of OOP and FP is both possible and useful
- promoted the adoption of strong static typing

### Aims:
- Make platform more powerful
- make the language simpler
- work on foundations to get to the essence of Scala

---

# Danese Cooper : **_Why Open Languages Win_**

- Slides unavailable online
- The "Open Source Diva"
- Distinguished Member of Technical Staff-Open Source at Paypal

---

# Danese Cooper : **_Why Open Languages Win_**

### Examples of how open sourced languages / tools out competed closed source rivals or forced them to go open source
- Java vs C++
- Apache/ servlets vs ASPs
- Apache Geronimo => Sun open sourced Glassfish
- Apache Harmony => Sun started OpenJDK
- S from Sass, led to R from academia
- Microsoft open sourced .NET
- Joyent did a bad job as "benevolent dictator"

---

# Danese Cooper : **_Why Open Languages Win_**

### Open source misteps
- SCSL - Sun Community Source License, not a good license, not open.
- Worked on Linux adoption at Intel, but windows desktop penetration too deep
- Joyent has done a bad job as "benevolent dictator" of Node.js leading to io.js fork

---

# Danese Cooper : **_Why Open Languages Win_**

### Take aways
- Open source is now a requirement to drive a language adoption
 - Don't try to monetize it
 - Have a permissive license
- It's quite possible to get it WRONG
 - Listen to your developers, they just want stuff to work
- Open Standards != Open Source
 - Lots of big companies will tell you otherwise
 - Open Standards isn't clearly defined like Open Source
 - Look Richard Stallman's 10 requirements for open source
 - Open Standards bodies are worried about De Facto standards

---

# Danese Cooper : **_Why Open Languages Win_**

### Q&A
- When to open source.  Answer these questions:
1.  Does anyone care?
2. Do we still use it (some companies tempted to OS junk they aren't using anymore)?
3. Is there a resource (so people can research it)?
4. If the first 3 things are yes, can we continue to work on the project after we open source it (modularize the "secret sauce" parts and keep them closed while working on the rest in the open)?

---

# Danese Cooper : **_Why Open Languages Win_**

### Q&A
- How do you finance open source?
- Dual license works for some projects (MySQL, MongoDB)
- Foundation is her favorite, keeps the books open and gives everyone a chance to contribute
- Sponsorship is hard to do well and leads to forks

---

# Dianne Marsh : **_Technical Leadership from wherever you are_**

- Director of Engineering Tools at Netflix
- [Slides](http://downloads.typesafe.com/website/presentations/ScalaDaysSF2015/Keynote_Marsh.pdf)
- Mostly motivational speech about being a leader
- Some specific advice
---

# Dianne Marsh : **_Technical Leadership from wherever you are_**
### Ways for technical managers to exercise technical muscle even when their primary job is to go to meetings all day

- Internal Hackathons
- Off critical path projects (not on any timeline, usually something like internal tools)
- Learn by listening - podcasts

---

# Dianne Marsh : **_Technical Leadership from wherever you are_**
## Types of Leaders and what they do
- Project leaders:
 - project management groups
 - follow through
 - communicate with team
---

# Dianne Marsh : **_Technical Leadership from wherever you are_**
## Types of Leaders and what they do
- People leaders:
 - give honest, frequent feedback
 - protect the company culture
 - help recruit coworkers
---

# Dianne Marsh : **_Technical Leadership from wherever you are_**
## Types of Leaders and what they do

- Idea Leaders:
 - Speak at conferences
 - Write
 - Organize Internal Events
---

# Dianne Marsh : **_Technical Leadership from wherever you are_**
## Types of Leaders and what they do
- Scala Leaders:
 - Be welcoming of newcomers
 - Recognize there's not Just One Way
 - Respect the journey - help new developers


---
class: center, middle
# Sessions I attended

---

# Scala Collections Performance
## Craig Motlin @motlin
### [Slides](http://downloads.typesafe.com/website/presentations/ScalaDaysSF2015/T1_Motlin_Scala_Collections_Performance.pdf)
---
# Scala Collections Performance

- Low level examination of performance of collections over data sets in the millions
- Goldman Sachs trader so exceptionally picky about performance
- They have their own open source collections library, gs-collections (written in java, tested in java/scala)
- Detailed comparisons between gs-c, scala mutable & immutable, (sometimes Java too)

---

# Life Beyond the Illusion of the Present
## Jonas Boner @jboner
### No slides
---
# Life Beyond the Illusion of the Present

- No code, philosophical selling of Reactive Manifesto
- Models of time in single processors break down when you need concurrency
- Transactions give you concurrency but don't distribute well
- Time is not a global present, it's relative to the observer and latency adds up
- Time is a series of causally related events
---
# Life Beyond the Illusion of the Present
- Immutability is a core requirement, data is FACTS
- Facts are not variable.  Accountants don't go back & change the books, they add new entries to reflect new information.
- CRUD => CR~~UD~~
- Descriptions of various consistency strategies and their costs

---
# Experiences Using Scala in Apache Spark
## Patrick Wendell, Databricks @pwendell
### [Slides](http://downloads.typesafe.com/website/presentations/ScalaDaysSF2015/T3_Wendell_Spark.pdf)

---
# Experiences Using Scala in Apache Spark

- Databricks is basically Spark as a Service
- View from a company switching to Scala
- Overall like it, they like the syntax and functional aspects
- They didn't like binary compatibility issues, tendency towards overly dense code and some other problems bad programmers can get themselvs into
---
# Experiences Using Scala in Apache Spark

- Releasing Databricks Scalaguide
- Example guidelines:
 - No symbolic names
 - Do not do monadic chaining (map, flatmap, get) more than 3 levels deep
- Enforced automatically with [Scala Style](https://github.com/scalastyle/scalastyle)
---
# Experiences Using Scala in Apache Spark
### Other notes
- Conjecture: most popular scala projects will hava Java APIs (due to bigger user base)
- Preferred IDE: IntelliJ IDEA
- Originally supported SBT and Maven, now Maven is their official build
 - Since they made that decision he prefers SBT now, due to maven's xml syntax and poor plugin format
- Book recommendation [Atomic Scala](http://www.atomicscala.com/)

---
# Type-level Programming in Scala 101
## Joe Barnes, Senior Software Architect at Mentor Graphics, @joescii
### [Slides](http://downloads.typesafe.com/website/presentations/ScalaDaysSF2015/T4_Barnes_Typelevel_Prog.pdf)
---
# Type-level Programming in Scala 101
- This talk blew my mind
- Very approachable introduction to type-level programming with excellent SMB2 metaphor
- Starts with reimplementing Boolean as type classes, progresses to implementing linked lists
---

# Happy Paths: Functional Constructs in the Wild
## Joe Walp, James Kionka
### No slides

---
# Happy Paths: Functional Constructs in the Wild

- Examples of how to migrate your team to start using Category Theory abstractions from Scalaz in a manageable way
 - Scalaz has `Maybe` type which is like `Option` but invariant instead of covariant (so you won't get a subtype) and doesn't have an unsafe `.get` method
 - Scalaz has Disjunction `\/` (not a V) which is similar to Scala's `Either` so you can get explicit exception types
- Overall there was a lot of category theory that went over my head
---

# Akka in Production: Why and How
## Evan Chan, Socrata Inc., @Evanfchan
### [Slides](http://www.slideshare.net/EvanChan2/akka-in-production-scaladays-2015)

---
# Akka in Production: Why and How

- Examples where he's used Scala and in particular Akka in production
- Introduces Stackable Actor traits - a nice way to wrap a receive block in an actor so you can layer in boilerplate functionality in a clean way (for things like logging and monitoring)

```scala
trait ActorStack extends Actor{
  def wrappedReceive: Receive
  def receive: Receive = {
    case x => (wrappedReceive orElse unhandled) x
  }
}
```

---
# Akka in Production: Why and How

```scala
trait Instrument1 extends ActorStack {
  override def receive: Receive = {
    case x =>
      println("before")
      super.receive(x)
      println("after")
  }
}
```

```scala
class DummyActor extends Actor with Instrument1 with Instrument2 {
  def wrappedReceive = {
    case "something" => println ("got something")
  }
}
```

---
# Akka in Production: Why and How
- How he gathers Akka performance metrics
 - Stack a trait that gathers time spent in receive block and message frequency
 - Uses `metricz` and exposes it with a Spray route, metrics service calls that route.
 - End result: pretty graphs
- Also showed how he traces Akka message flows, trAKKAr
- Overview of Backpressure - ability to tell senders to slow down/stop

---
# Akka in Production: Why and How
### Akka best practices
- Don't put things that can fail into Actor constructor
 - Supervisor will stop it (default strategy)
 - Use an initialization message
- Put Actor messages in companion object to control namespace
- Learn/use akka testkit
---
# The Scalactic Way
## Bill Venners
### [Slides](http://downloads.typesafe.com/website/presentations/ScalaDaysSF2015/T1_Venners_TheScalacticWay.pdf)

---
# The Scalactic Way
- Scalactic grew out of Scalatest
- Scalatest = quality through tests
- Scalactic = quality through types
- SuperSafe = quality through static analysis (free/premium library he's licensing)
---
# The Scalactic Way
- Collection of types called `AnyVals`- examples: `PosInt`, `PosZFloat`
- Use these instead of runtime `require(...)` checks
- At compile time `AnyVals` are replaced with their regular `Int`, `Double`... values.  No runtime performance hit!
- When types are guaranteed you can remove `assert` and `requires` all over your code
---
# The Scalactic Way

```scala
case class PropertyCheckConfig(
  minSize: Int = 100
) {
  require(minSize >= 0, "must be greater than zero")
}
```

```scala
case class PropertyCheckConfig(
  minSize: PosZInt = 100
)
```
---
# The Scalactic Way
- Types not always best solution
- Led to SuperSafe, static analysis, not a linter, a "scala subset policy enforcer"
- Also does not affect compiled binary (other than issues it causes you to fix)
---

# The Unreasonable Effectiveness of Scala for Big Data
## Dean Wampler @deanwampler
### [Slides](https://deanwampler.github.io/polyglotprogramming/papers/UnreasonableEffectivenessOfScalaForBigData.pdf)
---
# The Unreasonable Effectiveness of Scala for Big Data
- Hadoop great in 2008
- "Hadoop is the _Enterprise Java Beans_ of our time"
- Did a non-trivial map-reduce job in Hadoop, Scalding and Spark
- "Inverted Index" - web crawl a bunch of web pages and end up with a map where the keys are words in the pages and the values are lists of tuples of the files containing that word and the word count
---
# The Unreasonable Effectiveness of Scala for Big Data
- MapReduce job in Java - state of the art 2011/2012
 - Lots of overhead getting and setting properties and ceremony declaring types to set the code up
 - Actual algorithm you are doing is a small part
 - ~ 60 LOC
- MapReduce job in Scalding
 - Scalding is a scala wrapper around map reduce, by Twitter (based off of Cascading (Java))
 - ~20 LOC
---
# The Unreasonable Effectiveness of Scala for Big Data
### Shortcomings of Hadoop:
 - Only "batch" mode
 - Hadoop Storm for streaming mode, but you have to implement your algorithm a second time
 - Twitter released Summingbird, another scala wrapper over Scalding and Storm
 - Hadoop inefficient, unable to batch and cache jobs
---
# The Unreasonable Effectiveness of Scala for Big Data
### Spark example
- One nice api for batch and streaming mode
- Also works well for undistributed, small jobs.
- ~40 LOC, looks almost like vanilla Scala collections code
- "Scala has won big data"
 - Cloudera has acknowledged Spark as successor to Hadoop
 - All new tools coming out are written in Scala with Java API
---
# The Unreasonable Effectiveness of Scala for Big Data
### Mathematics libraries in scala
- Algebird
 - Aggregation abstract algebra
 - Can tune accuracy vs performance
 - Twitter's motto: "Hash, don't sample"
 - Algorithms that break down at Twitter's scale: Top K, Average, Max/Min
- Spire - powerful numerics library
---


# Akka HTTP:  The Reactive Web Toolkit
## Roland Kuhn, Akka Tech Lead at Typesafe, @rolandkuhn
### [Slides](http://downloads.typesafe.com/website/presentations/ScalaDaysSF2015/T1_Kuhn_Akka_Streams.pdf)

---
# Akka HTTP:  The Reactive Web Toolkit
### Akka Streams
- Akka implementation of [Reactive Streams](http://www.reactive-streams.org/) spec (others: JVM (RxJava,Slick), JavaScript, Network Protocols )
- Streams separate the What from the How (actors, in this case)
- You write your streams and then you need an `ActorFlowMaterializer` in addition to your `ActorSystem`
 - Other (unspecified) materializers to come (cluster deployment?)
- Impressive live code demo
---
# Akka HTTP:  The Reactive Web Toolkit
### Akka HTTP
- Akka HTTP is based off of Akka Streams
- This is Spray 2.0
- Experimental, but hinted at April/May release
- Still missing some Spray things like Http client, SSL integration, websockets
- Most of Spray DSL is the same, but the implementation is Stream based instead of Actor based
- Another impressive live code demo
---
# Akka HTTP:  The Reactive Web Toolkit

```scala
val routes = {
      pathPrefix("account") {
        (get & path(Segment)) { accountNum =>
          complete {
            lookupAccount(accountNum)
          }
        } ~
        ...
      }
    }
...
Http().bindAndHandle(routes, config.interface, config.port)
```
---
# Akka HTTP:  The Reactive Web Toolkit
### Akka HTTP
- Where it fits in:
 - `akka-cluster` and `akka-remote` between internal systems
 - `akka-http` to external systems
---
# Toward a Safer Scala
## Leif Wickland, Oracle  @leifwickland
### [Slides](http://downloads.typesafe.com/website/presentations/ScalaDaysSF2015/Toward%20a%20Safer%20Scala%20@%20Scala%20Days%20SF%202015.pdf)

---
# Toward a Safer Scala

- I saw this same talk at PNW Scala in November
- Highly recommended, has specific action items you can put in your code TODAY
- TL;DR

```scala
scalacOptions ++= Seq(
  "-Xlint",
  "-deprecation",
  "-Xfatal-warnings"
)
```
---
class: center, middle
# Trivia

---

# Trivia Questions for conference swag

## What language did Odersky create before Scala?

---
# Trivia Questions for conference swag

## What does the acronym `TASTY` stand for?

---
# Trivia Questions for conference swag

## Akka Http is ____ 2.0
---

# The End
## [My Notes](https://gist.github.com/gangstead/e0955e77864e318bc61e)
## Typesafe [presentation roundup](https://www.typesafe.com/blog/scala-days-san-francisco-presentation-roundup)
## Where are the videos, Typesafe?!

- Shameless Plug for NodeSchool
 - Next meetup 4/22
 - Express.js web framework
 - http://www.meetup.com/Nodeschool-Dallas/events/219510528/
