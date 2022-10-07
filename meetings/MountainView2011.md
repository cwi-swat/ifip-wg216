# Mountain View 2011

The zeroth meeting of the group will be held 1st&ndash;3rd June 2011, probably at Google in Mountain View, California, USA.
It may be relocated to downtown San Jose for logistical reasons.

Jan-Willem Maessen and Mark S. Miller are the hosts.


## Proposed Talks


### Communicating event-loop concurrency and distribution

Mark S. Miller and TomVanCutsem

Communicating event loops is the concurrency and distribution model that underlies both the E and AmbientTalk programming languages. The model is founded on actors, but unifies the concepts of actors with objects in ways that set it apart from earlier "active object" or actor languages. The goal of this talk is to give a general introduction to the model. As we are promoting these ideas for inclusion in future versions of Javascript, we will explain a proposed embedding of the model in Javascript.


### AmbientTalk: distributed object-oriented programming for mobile phones

TomVanCutsem (A short (30 min.) talk on AmbientTalk, the language I co-designed.)

AmbientTalk can best be summarized as "a scripting language for mobile phones". It's a dynamic, object-oriented, JVM-compatible, distributed programming language. AmbientTalk's focus is on applications to be deployed in so-called "mobile ad hoc networks" - networks of mobile devices that communicate peer-to-peer using wireless communication technology, such as WiFi or Bluetooth. We discuss how resilient mobile applications can be constructed with familiar building blocks like objects and messages, but also in what way these building blocks have to be adapted to fit the characteristics of mobile ad hoc networks.

Keywords: actors, event-driven programming, futures, remote objects, failure handling

### Ensō

William Cook (note, I have another meeting I have to go to afternoon June 2)

I'm currently designing a new programming/modeling language/system, called Ensō. I would love to get feedback, as I have not spoken publicly about it before. Depending on the level of interest, this talk might go for 30 minutes or much longer. Ensō shifts the focus from individual records or objects, toward a holistic view of data as connected graphs. Graphs are natural representation for data, including object models, grammars, business models, databases, state machines, web sites, graphical user interfaces, and types. The structure of a graph can be described/constrained by other graphs, which are analogous to types. Types in Ensō, which are checked dynamically, go beyond structural properties to include invariants and other meta-data. Ensō allows graphs to be easily created, stored textually, and manipulated graphically or programmatically. Ensō programs are transformations or interpretations of graphs. Example transformations are merge, difference, rendering one graph into the space of another graph, and parsing. These operations are generic, because they are parameterized by the description of the kind of data that they are to operate upon. Types are also graphs, so in addition to being checked, they can also be combined, merged, and generated dynamically. At the core of Ensō are a family of self-describing graphs. Ensō is constructed in itself, and is being used to create a family of applications, including a web application language, a diagram editor (GUI) among others. This is joint work with Tijs van der Storm (CWI).

### Batches: A unifying approach to remote execution, services, and database access

William Cook (note, I have another meeting I have to go to afternoon June 2)

This could be a very short talk, or a longer one. 15 to 45 minutes. I've given this talk a few times before, so I will not give it here unless people really want to hear it. It's about a finding a better way to do distributed objects. It also raises the question of how thousands of smart people could have persisted in making a huge mistake (CORBA/RMI/PRC/etc) in language design for over 30 years.

###  Combination of structure and behavior as an algebra

Erik Ernst

Very recently, a new advance was made towards the solution of an old problem in the language gbeta. The goal is to design classes/methods and combinations thereof in such a way that it always succeeds---even in cases where the classes/methods involved are not known statically---just like x+y always succeeds in the algebra of numbers with the operation '+'. One very persistent obstacle on this path is the fact that it breaks type safety to have a class that involves two different mixins with the same identity (same syntax) but different enclosing objects. This talk explains the overall problem of working towards this kind of safety, and in particular how one step in that direction has been invented and implemented recently.

### Await! Taking the misery out of asynchronous programming

Mads Torgersen

In the .NET and Windows world - as in most places - threads are precious, and we cannot afford to waste them doing idle waiting. UI's are generally single threaded, and server scaling is often bottle-necked by thread count. So in the age of networks and the cloud, where latency is rampant, using threads to do the waiting just doesn't scale.

People therefore - wisely - take to callback-based models of asynchronous programming. Unfortunately, manual wiring of callbacks at any scale is agonizing, error prone an unmaintainable: one of the world's least appetizing uses of first-class functions!

In the next versions of C# and Visual Basic we use a future-based metaphor for outstanding work - we call them Tasks - and let you directly "await" them in the language. This lets developers keep the natural flow of their imperative code, without magically hiding too much of what's really going on: A compromise in the old debate around transparency of distribution.

As a meta-point (which we can go into or not) C# async is representative of the form of "in the trenches" language design that is necessary when evolving industrially-adopted far-from-perfect languages under highly specific technical and target audience constraints. The human factor of language design takes on a certain acuteness when your end goal is to sell copies of Windows!

### Mutable state without imperative programming

Jonathan Edwards

Some day imperative programming will be seen as a barbaric practice from the stone age of software. Correctly sequencing myriads of memory accesses is a job for a compiler, not a human. Unfortunately imperative programming is still the only way we know for building programs with complex mutable state, a category that includes much application software. I am focusing on the problem of input processing in such applications. I propose to constrain the standard heap of objects and pointers into a special kind of tree structure. State mutation is constrained to an event driven pattern called hierarchical change-flow. These constraints enable the mutation of complex data structures to be programmed declaratively, that is, without sequential control flow.

### Toward a declarative foundation for compositional distributed programming

John Field

The distributed systems community has made enormous progress over the past few decades building specialized systems that scale to handle millions of users and petabytes of data. However, combining individual systems into composite applications that are scalable---not to mention reliable, secure, and easy to maintain---remains a challenge. This is where programming models should be able to help: good programming models are designed to facilitate composing large applications from smaller components, and for reasoning about the behavior of applications modularly. However, there appears to be relatively little work on defining appropriate linguistic foundations for large-scale distributed systems.

In this talk, I will describe the Reactor programming model, which is designed to serve serve as a foundation for building distributed applications in a declarative manner. A reactor consists of two principal components: mutable state, in the form of a fixed collection of relations, and code, in the form of a fixed collection of rules in the style of Datalog. Multiple reactors, which model nodes in a concurrent or distributed system, communicate with one another using actor-style messages. Rules are used to specify both local computations and inter-reactor communication.

A notable characteristic of distributed systems design is that applications must make explicit design choices among consistency, availability, and partition tolerance (Eric Brewer's "CAP" theorem). I will show through an extended example that tradeoffs in the CAP design space can be viewed as simple code refactorings in the Reactor model.

This work is joint with Maria-Cristina Marinescu and Christian Stefansen.

### Modularity & Visibility in Object-Oriented Languages

Kim Bruce

In the 1970’s and 80’s, there was incredible progress in the design of module systems for programming languages. Sadly, most of that work seems to have been forgotten in the last two decades. In particular, many users (and designers) of object-oriented languages have seemed to feel that classes could play the role of modules. We review some features of modules and propose a new module system for object-oriented languages that combines the information hiding and modularity of standard modules, with a notion of extension that fits the philosophy of object-oriented languages.

### Exploring the Web Programming Design Space

Eelco Visser

The web is the domain of polyglot programming. A typical web program requires HTML, CSS, JavaScript?, SQL, and your favourite GPL (Java, Scala, Ruby,...). All these languages are poorly integrated, giving rise to injection attacks and late detection of failures. With my students, I have been exploring the design space of linguistically integrated languages for web programming. WebDSL is a language for RESTful web applications and mobl is for stateful, client-side web applications, targeting mobile devices.

Instead of using a slide presentation, I would like to try talking about the language via code inspection. This would make it easier to have a conversation rather than a broadcast.

### Dimensions of Domain-Specific Language Design

Eelco Visser

The goal of domain-specific language engineering is to systematically design a DSL for a domain. But what makes a good language? For a while I have been asking colleagues the question: "What is a good language design?" Markus Voelter and I recently wrote a paper in which we attempt to answer the question. That is, we present a framework for describing and characterizing external domain specific languages. We identify eight design dimensions that span the space within which DSLs are designed: expressivity, coverage, semantics, separation of concerns, completeness, large-scale model structure, language modularization and syntax.

### Messages of Grace

James Noble

We are engaged in the design of a new object-oriented educational programming language called Grace. Our motivation is frustration with available languages, most of which are approaching 20 years old.

In this talk, I'll outline some principal features of Grace, discuss open issues, and listen to your reactions while all of the choices are still on the table. In particular, I'll give some examples from the design process so far, showing how conceptually orthogonal design decisions all too easily end up as tightly coupled gordian knots

### Karl Lieberherr was half-right: a personal history of Object Ownership

James Noble

An interactive historical ramble through nearly twenty years of research in object orientation: from Software Visualisation in Self via incredibly complex Object-Calculus encodings to the latest results rejected from OOPSLA!

(With pictures.)

I have to give this talk later in the year so I could get started now, but will not give it here unless people really want to hear it. I think this may be relevant to a couple of other talks, but I always think it may be relevant.

### We're all Postmodern Now.

James Noble

Another version of the postmodern talk that was quite fashionable about ten years ago. These days, Dick Gabriel and Guy Steele probably give better versions of this talk than I can manage.

This could be a very short talk, or a longer one. 15 to 150 minutes. At least half the talks above are explicitly postmodern in outlook, so people interested in the philosophical foundations might like this, but I've given versions of it a few times before, so I will not give it here unless people really want to hear it. Or we can discuss it in a bar after dinner.

Joint work with Robert Biddle, Carleton.

### Languages for Distributed Algorithms

Annie Liu

This talk describes a language for programming distributed algorithms, compilation of the language to generate actual implementations, and powerful optimizations that incrementalize expensive queries and remove unnecessary messages. The language does not embody new concepts but is powerful and simple for expressing distributed algorithms cleanly, free of implementation details. For example, Lamport's distributed mutual exclusion algorithm can be written in 30 lines, almost exactly like the pseudo code description of the algorithm, but with a precise semantics for execution. A best effort for programming this algorithm led to about 200 lines or more in C and Java, about 100 lines or more in Erlang and Python, and 90 lines in PlusCal, a nonexecutable specification language for specifying distributed algorithms (all numbers exclude comments and empty lines). Our compilation method allows such programs to be generated automatically. Our optimizations allow more efficient implementations to be derived systematically. We have successfully experimented with specifying and implementing a variety of well-known distributed algorithms, including Paxos and Byzantine Paxos for distributed consensus.

### Object Constructors in Grace

Andrew Black

I would like to talk about some of the challenges of designing Object Constructors in Grace. Why didn't we just copy Smalltalk or Java or Self? What are the desiderata for an object-oriented language that aims to be simple to explain and teach, to be as powerful as most existing languages, and to look forward to the world of manycore? Did we make the right compromises? And how does inheritance fit into the story?

### Matching Contexts

Robby Findler

Redex is a domain-specific language for writing, testing, and typesetting operational semantics (and related tasks). Linguistically, however, the most interesting part of Redex is its pattern matcher. More interesting, in fact, that we realized when we started working on it. Specifically, Redex's pattern language has a notion of context-sensitive matching, inspired by Felleisen/Hieb-style semantics. As it turns out, the precise semantics of context decomposition has not been nailed down anywhere and is pretty subtle.

This talk explores the design space for the semantics of the pattern matching and tries to bring across how rich it is, how to best make sense of decomposition as it is currently bring practiced, and how to design a programming language around it.

Joint work with Casey Klein, Steven Jaconette, Jay McCarthy

### Stop Fooling Around

David Ungar

It seems to me that most programming language 'research' is incremental. Is this a good thing? If not, what are the hard problems we want to be attacking? A language tends to optimize certain values at the expense of others, and thus the languages we design may be more context-dependent than we ever let on. Of course, I have a bit I can say from my perspective, but a discussion would be the main part. I would love to hear where each of us stand on these questions.

### Harnessing Emergence for Manycore Programming: Early Experience Integrating Ensembles, Adverbs,and Object-based Inheritance

David Ungar

This is a talk I gave at Onward 2010, about an attempt to get non-determinism and parallel ensembles into an object-oriented, Self-oidal language. The interesting part is that unintended consequences of the combination occurred for which I have no easy answers. If folks are interested, I would be happy to present the talk, and even happier to hear your thoughts. 
