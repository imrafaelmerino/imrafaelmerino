### Hi there 👋, my name is Rafael Merino
#### I am a functional programmer 👩‍💻

<img src="./banner_3.png" alt="logo"/>

Skills: JAVA / SCALA / CLOJURE / LISP / ERLANG / Functional Programming / Actors

- 📫 How to reach me: imrafaelmerino@gmail.com 
- 😄 Pronouns: he 
- ⚡ Fun fact: I was a chess ♔ player. I was the champion 🏆 of Spain 🇪🇸 several times during my childhood. 

List of my personal projects 💪 in chronological order and their making-of, sit back and grab 🍿:

- [json-values](https://json.values.imrafaelmerino.dev) 

<a href="https://github.com/imrafaelmerino/json-values"> <img src="logos/json_values_150x86.png" alt="json-values"/> </a>

This was my very first project as a functional developer 👏. I learned from [Rich Hickey](https://en.wikipedia.org/wiki/Rich_Hickey) how important persistent data 
structures are. By the time I started developing **json-values**, I was working with Json all the time. I really missed 
a persistent Json and a better API to manipulate them 😡. Developing **json-values**, I put into practice 🏋️‍ many new 
concepts for me like recursion, tail-call optimization, trampolines, high order functions, functors, monads, etc.

I started testing 🧪 **json-values** with a **Scala** library called [ScalaCheck](https://www.scalacheck.org), which is used for property-based testing (PBT).
This way, I killed two 🐦 with a stone; I learned a new language, **Scala**, and an inspiring testing philosophy. I discovered 
property-based testing thanks to [John Hughes](https://en.wikipedia.org/wiki/John_Hughes_(computer_scientist)) and [QuickCheck](https://hackage.haskell.org/package/QuickCheck) from Haskell. 
PBT led me to create a beautiful Json generator. I challenged the world, 
claiming it was the best Json generator in the whole galaxy 🌌 by that time (and still it is!) You can benefit from
this Json generator to test your code. Prove me wrong if you have a better alternative!

Spec is an incredible [Clojure](https://clojure.org) library. I implemented json-spec based on the ideas I learned from it. At the risk of being
presumptuous, I claim it's by far the best way of validating a Json in **Java** and **Scala**. It's easy to write, read, and 
maintain. Defining json generators and specs is a piece of 🍰.

I bought the book 📖 [Optics by example](https://leanpub.com/optics-by-example), from Chris Penner, written in **Haskell**. 
Good read, by the way. I studied [Monocle](https://www.optics.dev/Monocle/) in **Scala** as well. That allowed me to develop some optics in **json-values**. 
Since then, I use optics all the time.

Developing **json-values**, I started taming effects with FP. I experienced how great FP is describing, composing, and 
executing programs made up of effectful functions λ. I designed an interactive program that, given a spec, creates 
a Json asking the user for every value on the console 📺. I also wrote a Json future.

I developed json-values in **Scala** and **Dotty** as well. Dotty is a prerelease of Scala3.

  - [Java version](https://github.com/imrafaelmerino/json-values)
  - [Scala version](https://github.com/imrafaelmerino/json-scala-values)
  - [Dotty version](https://github.com/imrafaelmerino/json-dotty-values)

**Scala** is, in my option, a good alternative to do FP in the **JVM**. I've learned a lot from the **Scala** community. 
I have tremendous respect for the **Scala** creator, [Martin Odersky](https://en.wikipedia.org/wiki/Martin_Odersky), 
and the **ZIO** creator, [John A De Goes](https://degoes.net).
I never miss any of their talks and articles.

On the other hand, **Clojure** is a great choice as well. It's really challenging since it's a lispy programming language. 
As a **Lisp** fan, being able to use it in the **JVM** is incredible. You must see any talk from Rich Hickey. He made a significant impact 👊 on me, and he changed my life entirely as a programmer.
Being honest, it took me almost three years of my life to develop **json-values** and really understand functional programming. 
The **Scala** version took me only four months because I had already grasped the fundamentals.

**Java** doesn't have persistent data structures. **Scala** and **Clojure** does. This was a problem implementing 
the Java version of **json-values**. I tested a lot of alternatives and compare them in terms of performance and design.
I ended up using the persistent data structures from the library [vavr](https://www.vavr.io).  

- [vertx-effect](https://github.com/imrafaelmerino/vertx-effect)

<a href="https://github.com/imrafaelmerino/vertx-effect"> <img src="logos/vertx_effect_150x86.png" alt="vertx-effect"/> </a>

Suppose I had to describe **vertx-effect** in three words. In that case, they'd be without a doubt: expressions, composition, 
and persistent data structures or values. **vertx-effect** is the place where actors model meets functional programming
in **Java**.

I couldn't resist naming the most essential function in this library as lambda 😎

I had been working with Vertx for a long time. I always had the feeling that I could do it better 🤷‍♂️.
Asynchronous programming is hard. It's even harder if you have to deal with the callback hell 🔥 to do 
your business logic. Imperative programming doesn't help here. 

On the other hand, I started learning **Erlang** and watching videos of [Joe Armstrong](https://en.wikipedia.org/wiki/Joe_Armstrong_(programmer)). 
I read his [book](https://www.amazon.com/-/es/gp/product/B00I9GR4TW/ref=dbs_a_def_rwt_hsch_vapi_tkin_p1_i0) 📖  and [thesis](https://erlang.org/download/armstrong_thesis_2003.pdf).
I really understood the actor model and how powerful it is. I fell in love with failures 🤪. It's critical to know that 
every system will fail, and you'd better be prepared. Erlang uses persistent data structures, and so does **vertx-effect** 
thanks to **json-values** 👏

I learned from John A De Goes how to use FP to deal with effects. I took the course [Principles of Reactive Programming in Scala](https://www.youtube.com/playlist?list=PLMhMDErmC1TdBMxd3KnRfYiBV2ELvLyxN). 
The result is vertx-effect. There are some expressions implemented that come from **Lisp**, like Cond, Case, and IfElse.

It was sad to find out that Joe Armstrong had passed away † in 2019, a few months before I met him. Rest in peace, Joe. I strongly recommend you 
study his work. He was very brilliant and, at the same time, very kind and humble.

- [vertx-mongodb-effect](https://github.com/imrafaelmerino/vertx-mongodb-effect)

<a href="https://github.com/imrafaelmerino/vertx-mongodb-effect"> <img src="logos/vertx_mongodb_effect_150x86.png" alt="vertx-mongodb-effect"/> </a>

You can model any effect in **vertx-effect** using lambdas λ. **vertx-mondodb-effect** gives you some λ to interact 
with the **MongoDB**.
Going from Json to BSON and vice versa was really cumbersome and tedious. That's why I developed **mongo-values**, a set of 
codecs that abstracts you from that.

- [mongodb-values](https://github.com/imrafaelmerino/mongo-values)

**json-values** and **mongo-values** are ideal for working with MongoDB. **mongo-values** gives you a set of codecs that free the 
programmer from doing any kind of conversion to BSON.

- [JIO](https://github.com/imrafaelmerino/JIO)

<a href="https://github.com/imrafaelmerino/JIO"> <img src="logos/jio-150x86.png" alt="jio"/> </a>

**JIO is the proof you can do Functional Programming in Java 🕺**.  Values, expressions, and functions on top of the
CompletableFuture API. The **IO monad** is extremely powerful and allows you to tame any imaginable effect: console programs, 
HTTP requests, database calls, etc. Everything is composable and referential transparent in the world of lambdas λ and 
values, which helps you cope with complexity 😌. I think, nowadays (beginning of 2021), there's nothing compared to this 
in the Java world 🤷‍️.

I implemented a reactive MongoDB client and a reactive HTTP client. I developed some interesting console programs that
show the essence of JIO.

It's the first time I used **JFR** and **JMC**. I'm glad that since **Java 11**, we have these tools. Logging is a key aspect of any system.  

I fiddled with the fork/join framework that came out in **Java 7**. I thought you couldn't use it for blocking operations, but that's surprisingly false. 
The **ManagedBlocke**r interface opens the door to submitting blocking tasks to the pool, and I took advantage 💪 of this in JIO.

Since Mockito and all that stuff are not my cup of tea, I developed a native Java HTTP server to test my HTTP client.
Of course! The server is configurable just with functions.


[<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/twitter.svg' alt='twitter' height='40'>](https://twitter.com/imrafaelmerino)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/youtube.svg' alt='YouTube' height='40'>](https://www.youtube.com/channel/UCZi0p8cl-6VerKHh4u3FRog/featured)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/icloud.svg' alt='website' height='40'>](https://blog.imrafaelmerino.dev)  
