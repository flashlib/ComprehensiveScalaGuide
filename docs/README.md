What is Scala? | A Comprehensive Scala Tutorial
===============================================

by [DataFlair Team](https://data-flair.training/blogs/author/dfteam1/ "Posts by DataFlair Team") · Published March 24, 2018 · Updated December 26, 2018

1\. Scala Tutorial – Objective
------------------------------

We feel immense pleasure in welcoming you to yet another series of tutorials- Scala. What is Scala? What can you do with it? and What does it look like? These are some of the questions we will answer today in our comprehensive Scala tutorial. We will discuss what is Scala programming, Scala for beginners, history of Scala, Features of Scala, Frameworks of Scala, Applications of Scala, Companies that use Scala, and technologies that are built on Scala.

So, let’s begin with the Scala Tutorial.

[![What is Scala? | A Comprehensive Scala Tutorial](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2018/03/Scala-Tutorial-01-2.jpg)](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2018/03/Scala-Tutorial-01-2.jpg)

What is Scala? | A Comprehensive Scala Tutorial

2\. What is Scala Programming?
------------------------------

Scala is a portmanteau of ‘scalable’ and ‘language’. It is designed to grow with user demand.

A general-purpose programming language, Scala provides support for functional programming and a strong static type system.

Being much like [**Java Programming**](https://data-flair.training/blogs/java-tutorial/), Scala’s source code compiles into Java bytecode. The resulting executable code runs on a **[JVM (Java Virtual Machine)](https://data-flair.training/blogs/java-virtual-machine-jvm/)**. Actually, it supports language interoperability with Java. So, you can reference libraries written in both languages, in both of them. Other similarities between Java and Scala include an object-oriented nature and a curly-brace syntax.

However, unlike Java, Scala supports features of functional programming- like currying, type-inference, immutability, lazy evaluation, pattern matching, and nested functions. It also supports higher-order functions, where a function can return another, or take it as a parameter. Scala also has an advanced type system that supports algebraic data types, higher-order types, anonymous types, and covariance and contravariance.

Finally, Scala also allows functionality like operator overloading, raw strings, optional parameters, and named parameters. However, it doesn’t support checked exceptions, like Java does.

Hope now you are clear with **[reasons to why learn Scala](https://data-flair.training/blogs/why-scala/)**. Let us see a topic of Scala Tutorial: Scala History.

3. Scala Tutorial – History
---------------------------

Scala emerged on 20 January 2004, 14 years from now. While its design began in 2001 at the École Polytechnique Fédérale de Lausanne (EPFL) (in Lausanne, Switzerland) by Martin Odersky, it saw an internal release in late 2003. In 2004, it released to the public on the Java platform. Further, a second version followed in the March of 2006.

While Java adopted lambda expressions only in 2014, with Java, Scala always supported functional programming fully. On January 17th of 2011, the team for Scala bagged a five-year research grant of over €2.3 million from the European Research Council. Then, on May 12th of 2011, Odersky and collaborators launched Typesafe Inc., which they later renamed to Lightbend Inc. This was to provide commercial support, training, and services for Scala. In 2011, Greylock Partners invested $3 million in Typesafe.

4. Scala Tutorial – Features of Scala
-------------------------------------

Every language has some **[unique features](https://data-flair.training/blogs/scala-features-comprehensive-guide/)** which make them the best convenience of a particular type of Project.

In this Scala Tutorial, we have mentioned 14 such features of Scala Programming Language.

[![Features of Scala](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2018/03/Features-of-Scala-01.jpg)](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2018/03/Features-of-Scala-01.jpg)

Features of Scala

### a. Type Inference

Type inference means Scala automatically detects(infers) an expression’s data type fully or partially. We don’t need to declare it ourselves, and this also lets developers omit type annotations. This has no effect on the type checking.

The compiler checks the types of the subexpressions, or of atomic values like 42(Integer), and true(Bool). It aggregates this information to decide the type for the entire expression.

### b. Singleton Object

In Scala, you will see a **[singleton object](https://data-flair.training/blogs/scala-singleton-object/)** instead of static variables and methods. A singleton object is a class with a single object in the source file. To declare this, we use the ‘object’ keyword:

```
object Main extends App {
	println("Hello, World!")
}
```

### c. Immutability

Every time you declare a variable in Scala, it is immutable by default. This means you cannot modify it. But if you want, you may declare it as mutable. Then, it is possible to change its value.  
This property of Scala helps us with concurrency control.

### d. Lazy Evaluation

If declared lazy using the ‘lazy’ keyword, Scala delays complex computation with evaluating an expression until it absolutely needs it. We also call it call-by-need.

This avoids repeated evaluations. And these are the benefits of the same:

1.  Lazy Evaluation, lets us define control flow as abstractions instead of primitives.
2.  It lets us define potentially infinite data structures.
3.  It also improves performance.

Take an example:

```
lazy val images=getImages()
```

### e. Case Classes and Pattern Matching

A regular class that is immutable by default, and is decomposable via pattern matching, is a case class. Its parameters are public and immutable by default. We define a case class with the keywords ‘case class’, an identifier, and a parameter list which can be empty.

```
case class Book(isbn: String)
val frankenstein = Book("978-0486282114")
```

**[Scala Pattern matching](https://data-flair.training/blogs/scala-pattern-matching/)** allows us to compare a value against a pattern. This is like a switch-statement or a series of if-else statements in Java.

```
import scala.util.Random
val x: Int = Random.nextInt(10)
x match
{
	case 0 => "zero"
	case 1 => "one"
	case 2 => "two"
	case _ => "many"
}
```

Any doubt yet in Scala Programming Tutorial? Please Comment.

### f. Concurrency Control

The Actor model from Scala’s standard library lets us implement concurrency in code. Scala also has a platform/tool, Akka, which is a separate, open-source framework for Actor-based concurrency. It is possible to combine/distribute Akka’s actors with software transactional memory.

### g. String Interpolation

[**Scala String Interpolation**](https://data-flair.training/blogs/scala-string-interpolation/) is a form of template-processing. To interpolate a string is to evaluate a string literal consisting of one or more placeholders to yield a result. The corresponding values replace these placeholders.

String interpolation is observed in Scala since version 2.10.0. Three methods it offers for this are- s, f, and raw.

### h. Higher-Order Functions

Such functions can return another function, or take it as a parameter. Scala makes it possible by treating its functions as first-class citizens.

```
val salaries = Seq(20000, 70000, 40000)
val doubleSalary = (x: Int) => x * 2
val newSalaries = salaries.map(doubleSalary) // List(40000, 140000, 80000)
```

Here, map is a higher-order function.

Higher-order functions also let us implement function compositions and lambdas.

### i. Traits

A trait is a type holding certain fields and methods. We define traits using the ‘trait’ keyword:

```
trait Greeter
{
	def greet(name: String): Unit
}
```
You can think of it like a partially implemented interface. You can create a trait with abstract, and optionally, non-abstract methods, and can also combine multiple traits.

### j. Rich Set of Collections

The **[Scala library has a huge set of collection](https://data-flair.training/blogs/scala-sets/)**s with classes and traits to help collect data into an immutable or a mutable collection. The scala.collection.immutable package holds all immutable collections. They don’t allow us to modify data. Likewise, the scala.collection.mutable package holds all the mutable ones.

### k. Functional

Scala is a functional language and treats its functions as first-class citizens. It will let you create higher-order functions like we’ve discussed twice earlier in this article. Other than that, it also supports nested functions and methods and carrying. Currying is the act of translating the evaluation of a function that takes multiple arguments, into evaluating a sequence of functions, each with a single argument.

### l. Object-Oriented

**[Scala is object-oriented](https://data-flair.training/blogs/scala-object-oriented-programming/)** while also being functional. In it, every value is an object.

### m. Statically-typed

You usually won’t need to declare redundant type information in your code. Scala will decide that based on the types of subexpressions, or of atomic values. This is in pertinence to type inference.

### n. Extensibility

When you’re building domain-specific applications, you need domain-specific language extensions too. Scala delivers a combination of language mechanisms. Overall, it makes it easy to smoothly add new language constructs as libraries. Constructs like implicit classes and string interpolation help us do this; we don’t need meta-programming features like macros.

### o. Scala Runs on the JVM

Scala’s compiler converts the source into Java bytecode that runs on the JVM (Java Virtual Machine).

Next topic in Scala Tutorial is Frameworks for Scala.

5. Scala Tutorial – Frameworks for Scala
----------------------------------------

Which frameworks and development tools do we have with Scala? Let’s see.

[![Scala Frameworks](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2018/03/Frameworks-for-Scala-01.jpg)](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2018/03/Frameworks-for-Scala-01.jpg)

Scala Tutorial: Scala Frameworks

### a. Akka

https://akka.io/

A free and open-source toolkit and runtime, Akka simplifies constructing concurrent and distributed applications on the JVM. Akka is good with distributed processing.

### b. Apache Kafka

https://kafka.apache.org/

Kafka is an open-source stream processing software platform by the Apache Software Foundation. It is written in Scala and Java. From Kafka, you can expect a unified, high-throughput, low-latency platform for handling real-time data feeds. Kafka is good with distributed processing too.

**[Follow this link to know about Apache Kafka Tutorial](https://data-flair.training/blogs/apache-kafka-tutorial/)**

### c. ScalaQuery

scalaquery.org/

ScalaQuery is a low-level Scala API for database access, composable non-leaky abstractions, and compile-time checking and type-safety. The JDBC API is powerful but verbose.

### d. Squeryl

squeryl.org/

Squeryl is a DSL for manipulating database objects from within Scala. It is strongly-typed, declarative, and SQL-like.

### e. Lift

[https://liftweb.net/](https://liftweb.net/)

Lift is a free and open-source web framework for Scala. David Pollak created it because he was dissatisfied with some aspects of Ruby on Rails.

### f. Play!

[https://www.playframework.com/](https://www.playframework.com/)

An open-source web-application framework, Play! is written in Scala.

### g. Scalatra

scalatra.org/

Scalatra is yet another free and open-source web application framework that was written in Scala. It is an alternative to the Lift, Play!, and Unfiltered frameworks, and is a port of the Sinatra framework.

Next topic in Scala Tutorial is Applications of Scala.

6. Scala Tutorial – Applications of Scala
-----------------------------------------

So, what can we do with Scala? The following are just some of the things you can build with Scala:

1.  Android applications
2.  Desktop applications
3.  Concurrency and distributed data processing, for instance, Spark
4.  Front and back ends of web applications with scala.js
5.  Highly concurrent things, like messaging apps, with Akka
6.  Distributed computing; because of its concurrency capabilities
7.  Scala is used with [**Hadoop**](https://data-flair.training/blogs/hadoop-tutorial/); Map/Reduce programs
8.  **[Big Data](https://data-flair.training/blogs/bigdata-tutorial/)** and data analysis with Apache Spark
9.  Data streaming with Akka
10.  Parallel batch processing
11.  **[AWS lambda](https://data-flair.training/blogs/aws-lambda-tutorial/)** expression
12.  Ad hoc scripting in REPL

7\. What Companies Use Scala?
-----------------------------

[![Scala Tutorial - Companies using Scala](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2018/03/Companies-Use-Scala-01.jpg)](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2018/03/Companies-Use-Scala-01.jpg)

Scala Tutorial – Companies using Scala

*   Apple
*   Sony
*   Twitter
*   Netflix
*   LinkedIn
*   Tumblr
*   Foursquare
*   The Guardian
*   AirBnB
*   Precog
*   Klout
*   Meetup.com
*   Remember the Milk
*   The Swiss Bank UBS
*   Amazon
*   IBM
*   Autodesk
*   NASA
*   Xerox

We have mentioned few top companies that use Scala in this Scala Tutorial, but there are others as well.

8\. Hot Technologies That Were Built in Scala
---------------------------------------------

These big names made use of Scala:

*   [**Apache Spark**](https://data-flair.training/blogs/spark-tutorial/)
*   Scalding
*   Apache Kafka
*   Apache Samza
*   Finagle (by Twitter)
*   Akka
*   ADAM
*   Lichess

This was all on Scala Tutorial. Hope you are clear with What is Scala and it’s Scala overview

9. Scala Tutorial – Conclusion
------------------------------

So, in this Scala Tutorial, we have discussed Scala for beginners, what is Scala programming, Scala for beginners, history of Scala, Features of Scala, Frameworks of Scala, Applications of Scala, Companies that use Scala, and technologies that are built on Scala. This is just the beginning. Walk with us in our journey with Scala; it’s going to be fun!

**[Reference](https://en.wikipedia.org/wiki/Scala_(programming_language))**