### Hi there 👋, my name is Rafael Merino
#### I am a functional developer

<img src="./banner_3.png" alt="logo"/>

Skills: JAVA / SCALA / CLOJURE / LISP / ERLANG / Functional Programming / Actors

List of my personal projects 💪 in chronological order and their making-of, sit back and grab 🍿:

- [json-values](https://github.com/imrafaelmerino/json-values) 

<a href="https://github.com/imrafaelmerino/json-values"> <img src="logos/json_values_150x86.png" alt="json-values"/> </a>

This was my very first project as a functional developer 👏. 
I learned from [Rich Hickey]() how important persistent data structures are. 
By the time I started developing json-values, I was working with Json all the time. 
I really missed a persistent Json and a better API to manipulate them 😡. 
Developing json-values, I put into practice 🏋️‍ many new concepts for me like recursion, 
tail-call optimization, trampolines, high order functions, functors, monads, etc.

I started testing 🧪 json-values with a Scala library called ScalaCheck, which is used 
for property-based testing (PBT). This way, I killed two 🐦 with a stone; I learned 
a new language, Scala, and a new testing philosophy. I discovered [property-based testing]()
thanks to [John Huge](). PBT led me to create a beautiful Json generator. I challenged the world, 
claiming it was the best Json generator in the whole galaxy 🌌 by that time (and still it is!)
You can benefit from this Json generator to test your libraries. Prove me wrong if you 
have a better alternative!

Spec is an incredible Clojure library. I implemented json-spec based on the ideas I learned from Spec. 
At the risk of being presumptuous, I claim it's by far the best way of validating a Json in Java and Scala. 
It's easy to write, read, and maintain. Defining json generators and specs is a piece of cake 🍰.

I picked up a book in Haskell about optics from . Good read by the way. I studied Monocle in Scala as well.
That allowed me to develop some optics in json-values. I especially like Prisms to work with exceptions.
I use them all the time. 

Developing json-values, I started taming effects with FP. I experienced how great FP is describing, composing, 
and executing programs made up of _effectful_ functions. I designed an interactive program that creates a Json 
asking the user for every value on the console 📺. I also created a Json future. 


I developed json-values in Scala and Dotty as well. Dotty is a prerelease of Scala3.

  - [Java version](https://github.com/imrafaelmerino/json-values)
  - [Scala version](https://github.com/imrafaelmerino/json-scala-values)
  - [Dotty version](https://github.com/imrafaelmerino/json-dotty-values)
  
Scala is by far the best option to do FP in the JVM. I've learned a lot from the Scala community. 
I have tremendous respect for the Scala creator, [Martin Odersky](), and the [ZIO]() creator, [John A De Goes](). 
I never miss any of their talks and articles.

Clojure is a great alternative. It's really challenging since it's a _lispy_ programming language. 
As a [Lisp]() fan, being able to use it in the JVM is incredible. You must see any talk from Rich Hickey. 
He made a big impact on me, and he changed my life completely as a programmer.

Being honest, It's taken me almost three years of my life to develop json-values and to really understand
functional programming. The Scala version only four months, because I had already grasped the fundamentals. 

- [vertx-effect](https://github.com/imrafaelmerino/vertx-effect)

<a href="https://github.com/imrafaelmerino/vertx-effect"> <img src="logos/vertx_effect_150x86.png" alt="vertx-effect"/> </a>

If I had to describe vertx-effect in three words, they'd be without a doubt: expressions, composition and persistent
data structures or values. 

I can't resist to name lambda to the most important function in this library 🤷‍ 

I had been working with Vertx for a long time. I always had the feeling that I could do it better. Asynchronous
programming is hard. It's even harder if you have to deal with the callback hell to do your business logic.
Imperative programming doesn't help here. On the other hand, I started learning Erlang and watching videos
of Joe Armstrong. I red his book 📖 ----- and this thesis. I really understood the actor model and how powerful it is.
I fell in love with failures 🤪. It's key to understand that every system will fail, and you'd better be prepared.
Your first integration test should be to switch the router off 🔌 and check that your system is still up and running, and
it's telling you right away that there is no internet connection . Erlang uses persistent data structures and
so does vertx-effect thanks to json-values 👏

I learned from [John A De Goes]() how to use FP to deal with effects. I took the course [Reactive programming in Scala]().
The result is vertx-effect. There are some expressions implemented that comes from Lisp, like
Cond, Case and IfElse.  

It was sad to find out that Joe had passed away time before I met him. Rest in peace Joe. I strongly recommend you
study his work. He was very brilliant, but at the same time very kink and humble. 


- [vertx-mongodb-effect](https://github.com/imrafaelmerino/vertx-mongodb-effect)

<a href="https://github.com/imrafaelmerino/vertx-mongodb-effect"> <img src="logos/vertx_mongodb_effect_150x86.png" alt="vertx-mongodb-effect"/> </a>

Working with Vertx, you can model any effect with vertx-effect. vertx-mondodb-effect 
gives you some lambdas to interact with the Mongo database in a functional and 
reactive fashion. 

Going from Json to BSON and viceversa was really cumbersome and tedious. That0s why I developed
mongo-values, a set of codecs that abstracts you from that. 


- [mongodb-values](https://github.com/imrafaelmerino/mongodb-values)

json-values and mongo-values are ideal to work with MongoDB. mongo-values gives you a
set of codecs that free the programmer from doing any kind of conversion to BSON.

- 🔭 I’m currently working on JIO, zio-exp and migrating json-values into Kotlin. 
- 🌱 I’m currently learning Scala3 and STM 
- 👯 I’m looking to collaborate on anything challenging related to FP 
- 🤔 I’m looking for help with any of my projects 
- 📫 How to reach me: imrafaelmerino@gmail.com 
- 😄 Pronouns: he 
- ⚡ Fun fact: Lisp is the first functional programming language, and the second oldest programming language still in use 


[<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/linkedin.svg' alt='linkedin' height='40'>](https://www.linkedin.com/in/imrafaelmerino/)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/twitter.svg' alt='twitter' height='40'>](https://twitter.com/imrafaelmerino)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/youtube.svg' alt='YouTube' height='40'>](https://www.youtube.com/channel/imrafaelmerino)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/icloud.svg' alt='website' height='40'>](https://blog.imrafaelmerino.dev)  
