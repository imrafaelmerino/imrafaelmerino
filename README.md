### Hi there 👋, my name is Rafael Merino

#### I see myself as both a programmer 👩‍💻 and a relentless problem solver. Tackling tough challenges can make me feel like the most miserable person in the world—but the moment I solve them, I'm not the happiest person either 🤷. I simply move on, ready for the next challenge!

- 📫 How to reach me: imrafaelmerino@gmail.com
- 😄 Pronouns: he
- ⚡ Fun fact: I was a chess ♔ player. I was the champion 🏆 of Spain 🇪🇸 several times during my
  childhood.

Sit back and grab some popcorn 🍿 as I take you through a chronological journey of my personal
projects 💪:

## [json-values](https://github.com/imrafaelmerino/json-values)

This marked my initiation into the realm of functional programming 👏. Inspired by
[Rich Hickey](https://en.wikipedia.org/wiki/Rich_Hickey) and his emphasis on persistent data
structures, I embarked on creating **json-values**. Constantly immersed in JSON-related tasks, I
felt the need for a persistent Json structure and a more robust API for manipulation 😡. The
development of **json-values** became a playground for new concepts such as recursion, tail-call
optimization, trampolines, high-order functions, functors, and monads.

Testing 🧪 was a crucial aspect, and I explored the world of property-based testing (PBT) using the
**Scala** library [ScalaCheck](https://www.scalacheck.org). This not only introduced me to a new
language but also exposed me to a testing philosophy inspired by
[John Hughes](<https://en.wikipedia.org/wiki/John_Hughes_(computer_scientist)>) and Haskell's
[QuickCheck](https://hackage.haskell.org/package/QuickCheck). The outcome? A JSON generator I
proudly claimed to be the best in the galaxy 🌌, a challenge to which the world could respond with a
better alternative!

Spec, an incredible [Clojure](https://clojure.org) library, inspired me to create json-spec, a
validation approach I consider the best for **Java** and **Scala**. The process of defining JSON
generators and specs became a piece of 🍰. Additionally, I ventured into developing the fastest JSON
parser/validator in the JAVA ecosystem, adopting a novel approach of interleaving parsing and
validation for optimal performance.

My journey took me to the realm of optics through the book 📖
[Optics by example](https://leanpub.com/optics-by-example) by Chris Penner, written in **Haskell**.
Studying [Monocle](https://www.optics.dev/Monocle/) in **Scala** allowed me to incorporate optics
into **json-values**. Since then, optics have become an integral part of my toolkit.

The absence of persistent data structures in **Java** led me to explore and compare alternatives for
performance and design, ultimately choosing the vavr library for json-values.

---

## [vertx-values](https://github.com/imrafaelmerino/vertx-values)

In the Vert.x ecosystem, JSON message transmission is a prevalent practice, but challenges arise
when using of the native JsonObject or JsonArray types from Jackson due to the need for creating
copies, impacting performance and straining the Garbage Collector. **vertx-values** steps in as a
solution, leveraging the json-values framework to enable the transmission of immutable JSON objects.
vertx-values aims to significantly enhance the efficiency of JSON message transmission within Vert.x
applications.

---

## [mongodb-values](https://github.com/imrafaelmerino/mongo-values)

**json-values** and **mongo-values** form the perfect duo for seamless MongoDB interactions. With
**mongo-values**, programmers are liberated from manual BSON conversions, thanks to a set of codecs
that operate with exceptional speed. The process is streamlined – JSON is serialized and transmitted
over the wire, and vice versa for deserialization, eliminating the need for intermediate
conversions. This not only enhances performance but also simplifies the MongoDB workflow for
developers.

---

## [avro-spec](https://github.com/imrafaelmerino/avro-spec)

With the widespread popularity of Kafka, I opted to seamlessly integrate the json-values spec with
[Avro](https://avro.apache.org/), and the outcome is fantastic! **avro-spec** empowers you to create
[Avro](https://avro.apache.org/) schemas and serializers/deserializers with the
[specs](https://github.com/imrafaelmerino/json-values#specs) from json-values. Leveraging the
simplicity, intuitiveness, and composability of creating specs allows you to efficiently define Avro
schemas. The provided serializers/deserializers enable the transmission of the immutable and
persistent JSON from [json-values](https://github.com/imrafaelmerino/json-values) through the wire.

---

## [vertx-effect](https://github.com/imrafaelmerino/vertx-effect)

**vertx-effect in a Nutshell: The Fusion of Actors Model and Functional Programming in Java**

With an extensive background in Vertx, a persistent belief in doing better 🤷‍♂️ fueled my journey.
Asynchronous programming poses challenges, amplified in the daunting landscape of callback hell 🔥
for business logic. Imperative programming falls short, and while virtual threads are a boon, they
don't enhance program resilience. The crux lies in treating errors not as exceptions but as normal
data.

My revelation came while exploring **Erlang** and immersing myself in
[Joe Armstrong's](<https://en.wikipedia.org/wiki/Joe_Armstrong_(programmer)>) teachings through his
[book](https://www.amazon.com/-/es/gp/product/B00I9GR4TW/ref=dbs_a_def_rwt_hsch_vapi_tkin_p1_i0) 📖
and [thesis](https://erlang.org/download/armstrong_thesis_2003.pdf). The actor model's potency,
coupled with an appreciation for embracing failures 🤪, profoundly impacted **vertx-effect**,
enriched by persistent data structures from **json-values** 👏.

Inspired by John A De Goes, I embraced functional programming to tackle effects, drawing insights
from the
[Principles of Reactive Programming in Scala](https://www.youtube.com/playlist?list=PLMhMDErmC1TdBMxd3KnRfYiBV2ELvLyxN)
course. The resultant creation, **vertx-effect**, incorporates expressions like CondExp, SwitchExp,
and IfElseExp from **Lisp**.

A poignant note: The untimely passing † of Joe Armstrong in 2019 was a somber moment. His
brilliance, humility, and kindness continue to resonate through his enduring work, encouraging all
to delve into and appreciate his profound legacy.

---

## [vertx-mongodb-effect](https://github.com/imrafaelmerino/vertx-mongodb-effect)

You can express any effect in vertx-effect using Lambdas. With vertx-mongodb-effect, you gain access
to convenient Lambdas for seamless interaction with MongoDB, harnessing the power of mongo-values
and json-values.

---

## [JIO](https://github.com/imrafaelmerino/JIO)

JIO stands as a testament that Functional Programming in Java is more than just possible 🕺. It
seamlessly integrates values, expressions, and functions into virtual threads and structured
concurrency. The prowess of the IO monad unfolds, offering unparalleled capabilities to harness a
spectrum of effects, be it console programs, HTTP requests, or database calls. The world of lambdas
and values within JIO is inherently composable and referentially transparent, providing a robust
framework to navigate complexity 😌. In the realm of Java, there seems to be nothing quite like it
🤷‍️. JIO's expressive features are a tour de force in addressing complexity, and handling retries
with diverse policies becomes a straightforward task.

In my journey with JIO, I crafted a reactive MongoDB client and an agile HTTP client. I delved into
developing intriguing console programs that illuminate the core of JIO's capabilities.

Steering away from frameworks like Mockito, I engineered a native Java HTTP server to thoroughly
test my HTTP client. Remarkably, the server is entirely configurable using functions. Moreover,
leveraging virtual threads allows seamless conversion of any code into the JIO API. The jio-test
module further amplifies JIO's strength, enabling powerful property-based testing. Rest assured,
it's an effective tool for uncovering bugs in your code!

---

## [java-fun](https://github.com/imrafaelmerino/java-fun)

The primary objective of java-fun is to bring essential Functional Programming (FP) patterns to the
Java ecosystem. Unlike mere translations of these patterns from other languages, java-fun is
designed with the intent that any typical Java developer can effortlessly embrace and comprehend
these concepts. The emphasis is on preserving the essence of these patterns, ensuring developers do
not become entangled in unfamiliar types and conventions.

Here are the key concepts that have been thoughtfully implemented within java-fun:

- Pseudo Random Generators: Property-Based Testing is a highly effective testing approach, and
  having a robust set of generators that can be composed in countless ways is crucial. java-fun
  simplifies this process, making it incredibly straightforward.

- Optics: In functional programming, optics take precedence over traditional getters and setters.
  They offer safety and composability, eliminating the likelihood of encountering
  NullPointerExceptions when used correctly.

- Tuples: Although Java may not officially support tuples, they remain exceptionally valuable.
  java-fun introduces tuples with arities of two and three, encompassing pairs and triples,
  respectively. These structures enhance code expressiveness and maintainability.

---

## [javatudes](https://github.com/imrafaelmerino/javatudes)

"An étude (a French word meaning study) is an instrumental musical composition, usually short, of
considerable difficulty, and designed to provide practice material for perfecting a particular
musical skill." — Wikipedia

This project contains javatudes—Java programs, usually short, for perfecting particular programming
skills.

Admittedly, this idea isn't original; I borrowed it from Peter Norvig's Github repository. I simply
swapped Java for Python :)

Discover my Java solutions to the captivating Advent of Code. Dive into a plethora of puzzles and
algorithms, each meticulously solved without reliance on any external library. It's all about honing
skills, practicing, and, of course, having a great deal of fun along the way!

## [Mighty-Meter](https://github.com/imrafaelmerino/mighty-meter)

Mighty Meter is a streamlined solution for distributed performance testing using JMeter with
real-time monitoring powered by Grafana and InfluxDB. Easily set up in Docker, it enables scalable
testing and visualizes key metrics on intuitive dashboards to help you analyze and optimize
application performance at scale.

## [Kafka-CLI](https://github.com/imrafaelmerino/kafka-cli)

Kafka CLI is a powerful command-line interface tool designed to simplify and enhance your
interaction with Apache Kafka. Building on my expertise with JIO and the lessons learned from
developing avro-spec.
