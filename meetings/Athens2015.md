<div class="twikiTopic">
<h1 class="twikiTopicTitle">Meeting 2015</h1>
<div class="twikiWebTitle">Working Group on Language Design</div>
<ul>
<li> Dates: April 20-24 (Mon-Fri), 2015.
</li>
<li> Venue: Athens, Greece
</li>
<li> Host: Yannis Smaragdakis
</li>
</ul>
<p />
<h2><a name="Venue"> </a> Venue </h2>
<p />
The meeting will take place at the University of Athens Club (Kostis Palamas building).
<p />
The <a href="https://www.google.com/maps/place/Kostis+Palamas+Building/@37.980608,23.735297,17z/data=!3m1!4b1!4m2!3m1!1s0x14a1bd39be980c43:0x1e5f0b58a779ac73" target="_top">venue</a> is in downtown Athens, within a short walking distance of the Syntagma square (the modern center of town).
<p />
The building offers an array of options for internet access (guest access to the University network, eduroam) and a dining area for lunch. An all-day coffee and pastries buffet will be available throughout. Since laptop use during the meeting is discouraged, there will be a designated time period every day for laptop-detox (e.g., catching up and responding to urgent emails).
<p />
<h2><a name="Accommodation"> </a> Accommodation </h2>
<p />
There is an abundance of hotels in the area, at all price ranges. You should prefer the areas south of the meeting venue, where most of the hotels are anyway. See the attached map for the recommended area of your hotel search. Location-wise, you will be well-served by any of the ~100 hotels in the shown map area. Even the furthest away hotels on this map are within a half hour walk, or, equivalently, a 2-stop metro ride.
<p />
Sample picks:
<p />
<ul>
<li> Central Hotel (21 Apollonos St.): mid-range, good location for tourist areas, 1km to meeting venue.
</li>
<li> Amalia Hotel (10 Amalias Ave.): mid-range+, very central, next to Syntagma Square, quite close to meeting venue (&lt;1km).
</li>
<li> Divani Caravel (2 Vas. Alexandrou Ave.): mid-high range, a reliably high-quality Athens hotel, 2km to meeting venue.
</li>
<li> Titania Hotel (52 Panepistimiou Ave. not in the map area): well-known 4-star hotel, very close to meeting venue (0.5km).
</li>
<li> Grande Bretagne (Syntagma square): the top luxury hotel in downtown Athens, for those wanting to splurge. &lt;1km to meeting venue.
</li>
</ul>
<p />
<h2><a name="Registration"> </a> Registration </h2>
<p />
Registration is required, however fees will be collected at the meeting. Please register by emailing Dimitris Galipos: <a href="mailto:dgalipos@di.uoa.gr">dgalipos@di.uoa.gr</a>. Dimitris is in charge of all the meeting logistics.
<p />
The registration fee for the meeting is 180euros, which includes the cost for the all-day coffee buffet and lunch buffet for 5 days, as well as the cost of an excursion to the Acropolis. Dinners are not included--although we expect a planned group outing for dinner every evening, pricing and payment arrangements will be made on the spot.
<p />
<p />
    <img src="../pub/WGLD/Meeting2015/hotel-map2.jpg" alt="hotel-map2.jpg" width="800px"  />
<p />
<h2><a name="Registered"> </a> Registered </h2>
<p />
<ul>
<li> Gilad Bracha
</li>
<li> Edwin Brady
</li>
<li> James Cheney
</li>
<li> Adam Chlipala
</li>
<li> Jonathan Edwards
</li>
<li> Matthew Flatt
</li>
<li> Georgios Fourtounis
</li>
<li> Stefan Hanenberg
</li>
<li> Roberto Ierusalimschy
</li>
<li> Daan Leijen
</li>
<li> Jan-Willem Maessen
</li>
<li> Sean McDirmid
</li>
<li> Mark Miller
</li>
<li> James Noble
</li>
<li> Klaus Ostermann
</li>
<li> Nikolaos Papaspyrou
</li>
<li> Roly Perera
</li>
<li> Panagiotis Rondogiannis
</li>
<li> Kostis Sagonas
</li>
<li> Francisco Sant'anna
</li>
<li> Yannis Smaragdakis
</li>
<li> Ross Tate
</li>
<li> Sam Tobin Hochstadt
</li>
<li> Andrew Tolmach
</li>
<li> Tijs van der Storm
</li>
<li> Cristina Videira Lopes
</li>
</ul>
<p />
<h2><a name="Monday"> </a> Monday </h2>
<p />
<h3><a name="Sean_McDermid_Going_Against_the"> </a><a name="Sean_McDermid_Going_Against_the_"> </a> Sean McDermid: Going Against the Flow for Type-less Programming </h3>
<p />
Object-oriented languages are plagued by poor support for type inference given difficulty in combining subtype and parametric polymorphism. This talk will introduce a Type-less type system that provides useful type feedback about OO code with less type annotations. Type-less rethinks type checking as a modular field-aware value flow analysis to allow inference on assignment with simplified variance and binding. Type-less also does type inference backwards to specializes term types based on their usage rather than generalizing types to validate their usage. Type annotations are then unnecessary in client code that does not define new abstractions, and greatly reduced otherwise. The result is a fluid programming experience whose feel approaches that of a dynamic language, which I will demo, of course!
<p />
<p />
<h3><a name="Adam_Chlipala_The_Ur_Web_People"> </a><a name="Adam_Chlipala_The_Ur_Web_People_"> </a> Adam Chlipala: The Ur/Web People Organizer: A Library for Rapid Development of Web Apps from Components </h3>
<p />
I'll introduce a new library for the Ur/Web programming language that I talked about at past meetings of this group.  Ur/Web has some novel features that support unusual and effective styles of encapsulation; I'll review those a bit.  The purpose of the talk, which will focus heavily on code demos, is the new library, the Ur/Web People Organizer, which is based on a component architecture that allows very rapid assembly of applications for running meetings, etc.  A growing set of components encapsulate such ideas as scheduling meetings between two groups of people, taking RSVPs for different subevents, etc.  Each component has a rich static type, expressing its polymorphic dependencies on the schemas of selected SQL database tables.
<p />
<p />
<h3><a name="Markus_V_lter_Experiences_from_b"> </a> Markus V�lter: Experiences from building mbeddr </h3>
<p />
Over the last four years a team at fortiss and itemis have built mbeddr,
an extensible set of integrated languages for embedded software
development. mbeddr relies on the <span class="twikiNewLink" style='background : #FFFFCE;'><font color="#0000FF">JetBrains</font><a href="https://program-transformation.org/edit/WGLD/JetBrains?topicparent=WGLD.Meeting2015"><sup>?</sup></a></span> MPS language workbench. MPS'
projectional editor enables wide-ranging language modularity and
flexible notations that include text, prose, tables, mathematics and
diagrams. As far as we know, mbeddr is the largest and most
sophisticated system built on top of a projectional language workbench.
In this talk I will <strong>very briefly</strong> show mbeddr and recap the 'mbeddr
experience'. In particular, I will point out the problems we had to
fight with during mbeddr's construction, including those created by MPS
as well as those that resulted from our own ignorance. I will close the
talk by indentifying some of the areas in which MPS could be (or is
currently being) improved: some of them are certainly interesting topics
for academic research.
<p />
<h3><a name="Roberto_Ierusalimschy_Integers_i"> </a> Roberto Ierusalimschy: Integers in Lua </h3>
<p />
Numerical support in programming languages is not a very glamorous
subject. Nevertheless, it is a fundamental aspect of any language, and
things are far from settled. Each new programming language comes with an
almost unique set of number representations and sizes, coercion rules,
overflow handling, etc.
<p />
Lua, unlike most other programming languages, offered only one numerical
representation, (double-precision) floating-point numbers. This approach
simplifies the language and also its implementation, and for many years
served the needs of the language.
<p />
However, in recent years, two trends changed that situation. One is
the spread of 64-bit machines, and with it the spread of 64-bit APIs,
algorithms, etc. The other is the increased embedding of Lua in small
devices and its use in the "Internet of Things". As a result, after much
deliberation, Lua 5.3 (released Jan 2015) has incorporated (64-bit)
integers.  In this talk, I will discuss the process that led to this
change.
<p />
<h3><a name="Matthew_Flatt_Binding_as_Sets_of"> </a> Matthew Flatt: Binding as Sets of Scopes </h3>
<p />
Hygienic macro expansion is usually described as a kind of translation
into lexical-scope machinery. In particular, variables must be
"renamed" to match the mechanisms of lexical scope as the variables
interact with macros. In a new macro expander for Racket, we discard
the renaming approach and start with a generalized idea of "macro
scope", where lexical scope is just a special case of macro scope when
applied to a language without macros. The resulting macro system has
slightly different properties than the old one, but purely
pattern-based macros work as before, and the vast majority of macros
in existing Racket code also continue to work. At the same time, the
macro system is easier to explain and specify than one based on
renaming. The corresponding implementation is simpler, and it avoids
bugs that have proven too difficult to repair in the current macro
expander.
<p />
<p />
<h3><a name="Yannis_Smaragdakis_Streams_a_la"> </a><a name="Yannis_Smaragdakis_Streams_a_la_"> </a> Yannis Smaragdakis: Streams a la Carte: Extensible Pipelines with Object Algebras </h3>
<p />
Streaming libraries have become ubiquitous in object-oriented languages, with recent offerings in Java, C#, and Scala. All such libraries, however, suffer in terms of extensibility: there is no way to change the semantics of a streaming pipeline (e.g., to fuse filter operators, to perform computations lazily, to log operations) without changes to the library code. Furthermore, in some languages it is not even possible to add new operators (e.g., a zip operator, in addition to the standard map, filter, etc.) without changing the library.
<p />
We address such extensibility shortcomings with a new design for streaming libraries, based on treating the library as a domain-specific language interpreter. The architecture underlying this design borrows heavily from Oliveira and Cook�s object algebra solution to the expression problem, extended with a design that exposes the push/pull character of the iteration, and an encoding of higher-kinded polymorphism. We apply our design to Java and show that the addition of full extensibility is accompanied by high performance, matching or exceeding that of the original, highly-optimized Java streams library.  
<p />
<p />
<p />
<h3><a name="Jonathan_Aldrich_On_the_Evaluati"> </a> Jonathan Aldrich: On the Evaluation of Language Designs </h3>
<p />
How does one evaluate a language design?  Clearly there are multiple modalities, including case studies, human subjects experiments, benchmarking, code corpus studies, observational studies, etc.  What are the strengths and drawbacks of each?  Are there examples of each in the literature that we find exemplary?  I will lead a structured discussion aimed at coming to a preliminary consensus on some principles at the meeting, and identifying a subgroup interested in turning the results into a paper.
<p />
<p />
Because I am interested in starting an ongoing discussion, I would be interested in giving my talk relatively early in the week.  For example, I will be prepared to give it the first day, if scheduling permits.
<p />
<h2><a name="Tuesday"> </a> Tuesday </h2>
<p />
<h3><a name="Andrew_Tolmach_A_Theory_of_Name"> </a><a name="Andrew_Tolmach_A_Theory_of_Name_"> </a> Andrew Tolmach: A Theory of Name Resolution </h3>
<p />
Joint work with Pierre Neron, Eelco Visser and Guido Wachsmuth
<p />
We describe a language-independent theory for name binding and resolution, suitable for programming languages with complex scoping rules including both lexical scoping and modules. We formulate name resolution as a two stage problem. First a language-independent scope graph is constructed using language-specific rules from an abstract syntax tree. Then references in the scope graph are resolved to corresponding declarations using a language-independent resolution process. We introduce a resolution calculus as a concise, declarative, and language-independent specification of name resolution. We develop a resolution algorithm that is sound and complete with respect to the calculus. Based on the resolution calculus we develop language-independent definitions of alpha-equivalence and rename refactoring.
<p />
<h3><a name="Klaus_Ostermann_Language_Design"> </a><a name="Klaus_Ostermann_Language_Design_"> </a> Klaus Ostermann: Language Design by Duality: Making defunctionalization and refunctionalization symmetric </h3>
<p />
Reynold's defunctionalization and Danvy's refunctionalization
establish a correspondence between programming with first-class
functions and programming with pattern matching, but the
correspondence is not symmetric: Not all uses of pattern
matching can be automatically refunctionalized to uses of
higher-order functions. This asymmetry makes it hard to compare
the two styles of programming or convert automatically between
them. We generalize from first-class functions to arbitrary
codata. This leads us to a pair of languages, one with codata
support based on Abel's copattern matching and one with data
support based on pattern matching. They support full
defunctionalization and refunctionalization.
<p />
<h3><a name="Panagiotis_Rondogiannis_Extensio"> </a> Panagiotis Rondogiannis: Extensional Higher-Order Logic Programing </h3>
<p />
We present a purely extensional higher-order logic programming
language. In this language predicates denote sets, and two predicates
are  equal iff they are equal as sets. Moreover, every program has a
unique minimum Herbrand model which is the greatest lower bound
of all Herbrand models of the program and the least fixed-point
of an immediate consequence operator. In other words, we provide
a purely extensional theoretical framework for higher-order logic
programming which generalizes the familiar theory of classical
(first-order) logic programming. We discuss an extension of the
language which supports negation-as-failure, and present its
semantics.
<p />
<h3><a name="Francisco_Sant_anna_Structured_S"> </a> Francisco Sant'anna: Structured Synchronous Reactive Programming with C�u </h3>
<p />
Structured synchronous reactive programming (SSRP) augments classical
structured programming (SP) with continuous interaction with the environment.
We advocate SSRP as viable in multiple domains of reactive applications and
propose a new abstraction mechanism for the synchronous language C�u:
Organisms extend objects with an execution body that composes multiple
lines of execution to react to the environment independently.
Compositions bring structured reasoning to concurrency and can better describe
state machines typical of reactive applications.
Organisms are subject to lexical scope and automatic memory management similar
to stack-based allocation for local variables in SP.
We show that this model does not require garbage collection or a "free"
primitive in the language, eliminating memory leaks for organisms by design.
<p />
<p />
<h3><a name="Sam_Tobin_Hochstadt_Pycket_a_tra"> </a> Sam-Tobin Hochstadt: Pycket, a tracing JIT compiler for a functional language. </h3>
<p />
<h3><a name="James_Cheney_Teaching_about_PL_D"> </a> James Cheney: Teaching (about) PL Design (Discussion) </h3>
<p />
My department's previous courses on functional programming and operational semantics saw dwindling participation recently, leaving an unsightly gap between the FP and OOP basics covered in the first two years and the advanced courses taught in the fourth year.  I am currently facing the challenge (and opportunity) of developing a new PL course aimed at 3rd year students, to fill this gap.  
<p />
Following internal discussion, my current plan is to make language design considerations ("good", "bad", tradeoffs) a unifying theme of the course, and placing greater weight on practical experience (interpreters, DSL implementation) and less on foundations (operational semantics, specification, etc.) than our previous courses.  
<p />
My totally selfish goal in this talk/discussion is to present the context motivating my current plan and provoke the audience into helping me refine and improve it; less selfishly I hope this will also lead to some transferable insights or ideas about how to make PL ideas (including the notion of, and evaluation/appreciation of PL designs, not just isolated features or "paradigms") a central selling point of a flagship PL course.  If not,  then at least it will be an amusing exercise for the other WGLD participants to poke holes in my current plan.
<p />
<p />
<h2><a name="Wednesday"> </a> Wednesday </h2>
<p />
<p />
<h3><a name="Edwin_Brady_Uniqueness_Types_in"> </a><a name="Edwin_Brady_Uniqueness_Types_in_"> </a> Edwin Brady: Uniqueness Types in Idris </h3>
<p />
I will present a newly implemented feature in the Idris programming language, Uniqueness Types, and show how they can be used in practice to implement programs with compile time guarantees on resource usage. They are inspired by a similar feature in the Clean programming language, and by Ownership Types in Rust.
<p />
A value with a uniqueness type can be used at most once in a program. This means that once used, the memory they occupy can be safely reallocated. Furthermore, it becomes possible to represent and reason about state machines directly in types. I will discuss some of the trade-offs in the design and present a practical example, namely type-safe concurrent programming.
<p />
<p />
<h3><a name="Sophia_Drossopoulou_Pony"> </a> Sophia Drossopoulou: Pony </h3>
<p />
The language Pony was developed with the aim to support easy concurrent programming, fast implementations, and data-race freedom.
<p />
In terms of case studies and benchmarks, we argue that indeed, Pony programs are fast. In terms of our and our collaborators� programming experience, we argue that Pony is easy to learn and program in. We then outline some salient features of the Pony type system, and the garbage collection system.  
<p />
<p />
<p />
<h3><a name="Kostis_Sagonas_Type_Inference_ba"> </a> Kostis Sagonas: Type Inference based on Success Typings for Erlang: A Success? </h3>
<p />
Erlang is a concurrent functional programming language designed by Ericsson to meet the needs of developing large-scale telecommunication systems.  It has been designed as a dynamically typed but type safe language.  For more than ten years now, Erlang is coming with static analysis tools that perform aggressive type inference based on success typings and a language for optional type declarations and function specifications.  In this talk we will try to discuss whether this approach to adding types to a language designed to be dynamically typed was a good or a bad one and the lessons that have been learned in the process.
<p />
<h3><a name="Excursion_to_Acropolis"> </a> Excursion to Acropolis </h3>
<p />
After lunch we leave for an afternoon at the Acropolis
<p />
<h2><a name="Thursday"> </a> Thursday </h2>
<p />
<p />
<h3><a name="Gilad_Bracha_Implementing_Access"> </a> Gilad Bracha: Implementing Access Control In Newspeak </h3>
<p />
(joint work with Ryan Macnak)
<p />
There is a natural affinity between object-based encapsulation and capability-based security.  The Newspeak programming language capitalizes on this affinity.  However, until recently Newspeak did not enforce access control. This is changing, and provides a clean basis for building a secure, object-capability based system.
<p />
I�ll discuss the Newspeak access control semantics and our ongoing experience in implementing and using them.
<p />
<p />
<h3><a name="Roly_Perera_Demand_indexed_compu"> </a> Roly Perera: Demand-indexed computation </h3>
<p />
I'll talk about an idea that came out of the work on program slicing
that I did for my <span class="twikiNewLink" style='background : #FFFFCE;'><font color="#0000FF">PhD</font><a href="https://program-transformation.org/edit/WGLD/PhD?topicparent=WGLD.Meeting2015"><sup>?</sup></a></span>.
<p />
An important role of GUIs is to provide control over the <em>demand</em> active
on the output of a computation, via widgets like scrollpanes,
collapsible lists, and tooltips. This usually means computing all the
output upfront and then hiding some of it, or computing it as needed
using ad hoc, application-specific logic.
<p />
A somewhat independent observation is that pattern-matching imposes a
demand on the thing being pattern-matched: for example a function
defined by a set of equations needs to know something (but typically not
everything) about the argument in order to decide which of its defining
equations is applicable.
<p />
"Tries" (a.k.a. prefix trees), extended with a notion of variable
binding, can be used to formalise both of these notions of demand. I'll
outline an operational semantics for a simple functional language where
the demand on the output is specified explicitly in the form of a trie
of a suitable type. Running the same program with more demand produces
correspondingly more output. I plan to extend this with a notion of
"differential" trie, representing a change in demand, plus a
differential operational semantics which, given an increase in demand,
does just enough extra work to produce the required extra output.
Although I haven't worked this bit out yet, I'll try to explain the idea
with several examples.
<p />
<h3><a name="Ross_Tate_Collaborating_with_Cey"> </a> Ross Tate: Collaborating with Ceylon and Kotlin </h3>
<p />
I have been collaborating with the Ceylon team at Red Hat and the Kotlin team at <span class="twikiNewLink" style='background : #FFFFCE;'><font color="#0000FF">JetBrains</font><a href="https://program-transformation.org/edit/WGLD/JetBrains?topicparent=WGLD.Meeting2015"><sup>?</sup></a></span> for approximately 4 years now. In these collaborations, I have not designed any languages; rather I have helped these teams make their designs have the properties that they want. In this process, I have come to understand their underlying design philosophies, many of which are motivated by their development experiences as well as what they perceive to be necessary for industry adoption. I will present my personal understanding of their perspectives, while focusing on aspects that may generalize to other industry language designs. Whether those aspects actually generalize will hopefully prompt lively discussion.
<p />
<h3><a name="Tijs_van_der_Storm_Demo"> </a> Tijs van der Storm: Demo </h3>
<p />
<h3><a name="Crista_Lopes_Big_Code_What_we_ca"> </a> Crista Lopes: Big Code: What we can learn and What we can do </h3>
<p />
I will give an account of my 9-year work on mining large repositories of code towards the goal of producing the ultimate "do what I mean" programming environment. I will cover the lessons learned, both positive and not-so-positive. These lessons raise some interesting questions for programming language design.
<p />
<h3><a name="Business_Meeting"> </a> Business Meeting </h3>
<p />
For members
<p />
<h2><a name="Friday"> </a> Friday </h2>
<p />
<h3><a name="Eelco_Visser_Dynamic_Semantics_S"> </a> Eelco Visser: Dynamic Semantics Specification in DynSem </h3>
<p />
In this talk I demonstrate the design of the DynSem language for the specification of dynamic semantics. From DynSem specifications we generate interpreter implementations in Java, which are integrated in the IDE for the object language generated by the Spoofax Language Workbench.
<p />
<h3><a name="James_Noble_Swapsies_on_the_Inte"> </a> James Noble: Swapsies on the Internet - First Steps towards Reasoning about Risk and Trust in an Open World </h3>
<p />
Contemporary open systems use components developed by many different
parties, linked together dynamically in unforeseen
constellations. Code needs to live up to strict security
specifications: it has to ensure the correct functioning of its
objects when they collaborate with external objects of unknown
provenance, and it has to protect its objects� integrity even when
external objects are malicious.
<p />
In this talk we propose specification concepts to model risk and trust
in such open systems. We use these concepts to specify the
escrow exchange example, and discuss the meaning
of such a specification.
We'll argue informally that the code satisfies its specification
<p />
<h3><a name="Stefan_Hanenberg_Discussion_on_E"> </a> Stefan Hanenberg: Discussion on Empirical Methods </h3>
<p />
"How do different empirical methods interact? And why do I (still) vote for ignoring qualitative research?"

</div>
