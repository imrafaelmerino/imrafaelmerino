### Hi there 👋, my name is Rafael Merino
#### I identify as both a programmer 👩‍💻 and a problem solver. The moments of struggle in solving a problem make me feel like the most miserable person in the world. Conversely, the joy of successfully overcoming a challenge doesn't make me the happiest person 🤷; instead, I simply move on to the next problem.


<img src="./banner_3.png" alt="logo"/>

- 📫 How to reach me: imrafaelmerino@gmail.com 
- 😄 Pronouns: he 
- ⚡ Fun fact: I was a chess ♔ player. I was the champion 🏆 of Spain 🇪🇸 several times during my childhood.


Sit back and grab some popcorn 🍿 as I take you through a chronological journey of my personal projects 💪:

- [json-values](https://json.values.imrafaelmerino.dev) 

<a href="https://github.com/imrafaelmerino/json-values"> <img src="logos/json_values_150x86.png" alt="json-values"/> </a>

This marked my initiation into the realm of functional programming 👏. Inspired by [Rich Hickey](https://en.wikipedia.org/wiki/Rich_Hickey) and his emphasis on persistent data structures, I embarked on creating **json-values**. Constantly immersed in JSON-related tasks, I felt the need for a persistent Json structure and a more robust API for manipulation 😡. The development of **json-values** became a playground for new concepts such as recursion, tail-call optimization, trampolines, high-order functions, functors, and monads.

Testing 🧪 was a crucial aspect, and I explored the world of property-based testing (PBT) using the **Scala** library [ScalaCheck](https://www.scalacheck.org). This not only introduced me to a new language but also exposed me to a testing philosophy inspired by [John Hughes](https://en.wikipedia.org/wiki/John_Hughes_(computer_scientist)) and Haskell's [QuickCheck](https://hackage.haskell.org/package/QuickCheck). The outcome? A JSON generator I proudly claimed to be the best in the galaxy 🌌, a challenge to which the world could respond with a better alternative!

Spec, an incredible [Clojure](https://clojure.org) library, inspired me to create json-spec, a validation approach I consider the best for **Java** and **Scala**. The process of defining JSON generators and specs became a piece of 🍰. Additionally, I ventured into developing the fastest JSON parser/validator in the JAVA ecosystem, adopting a novel approach of interleaving parsing and validation for optimal performance.

My journey took me to the realm of optics through the book 📖 [Optics by example](https://leanpub.com/optics-by-example) by Chris Penner, written in **Haskell**. Studying [Monocle](https://www.optics.dev/Monocle/) in **Scala** allowed me to incorporate optics into **json-values**. Since then, optics have become an integral part of my toolkit.

While the initial development of **json-values** occurred in **Scala** for the sheer joy of it, I recognized the need for dual versions:
- [Java version](https://github.com/imrafaelmerino/json-values): Implemented using persistent data structures from [vavr](https://www.vavr.io).
- [Scala version](https://github.com/imrafaelmerino/json-scala-values): Developed for fun, though not actively maintained.

The absence of persistent data structures in **Java** led me to explore and compare alternatives for performance and design, ultimately choosing the vavr library.

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


- [java-fun](https://github.com/imrafaelmerino/java-fun)

Best API in Java to do Property Based Testing.

[<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/twitter.svg' alt='twitter' height='40'>](https://twitter.com/imrafaelmerino)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/youtube.svg' alt='YouTube' height='40'>](https://www.youtube.com/channel/UCZi0p8cl-6VerKHh4u3FRog/featured)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/icloud.svg' alt='website' height='40'>](https://blog.imrafaelmerino.dev)  
