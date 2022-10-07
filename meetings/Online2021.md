# WG2.16 online meeting June 7-11, 2021


We plan each day to have two 50 minute talks, including Q&A. Discussions can continue after the scheduled end of session.

Slots in Amsterdam time: every day 20:00-20:50, 21:10-22:00

Tentative schedule:
- Monday: Sean, Matthias
- Tuesday: Jan-Willem, James
- Wednesday: Francois, Jonathan A.
- Thursday: Tijs, Joe
- Friday: John, Luke


As per our Chatham House Rule, we ask that no one make recordings.

## Talks

### Luke Church - Phenomenology, aesthetics and identity politics in PL design

Some programming ecosystems feel ‘right’, and ‘enjoyable’ places to work in. Others feel like spaces of bureaucratic [and other forms] of assault on our work and our lives. In interviews with both programmers and programming language designers, an instinct of how things feel, what is ‘right’ in a design and what is ‘the thing that professionals should do’ have a significant impact on design that can’t and shouldn’t be reduced to ‘usability’.

I’m exploring a tentative lens of phenomenology (how things feel), aesthetic preference (what is prefered) and identity politics (what is the thing that you should do as a ‘modern programmer’) to describe how decisions get made in design, and if we can bring these hidden forces to the surface what would that mean for designing languages and systems?

This is early work that I’d love to try and explain to WGLD and see what happens, what parts of it make sense, which parts resonate and which you disagree with

### Sean McDirmid - Compositional reasoning in testing


Unit tests exercise module code against an informal specification that stands on its own. Because unit test results do not “integrate” at all, integration tests, which are much less effective in stressing module code paths, must fill in the gaps. I’m currently exploring how to “fix testing” with compositional reasoning as inspired by type systems. There is a duality between a module’s unit tests that ensure it is internally correct and the mocks and fakes that replicate the module’s behavior to represent its external use in the unit tests of other client modules. If we can encode a module’s unit tests and their mocks/fakes together, unit test results for multiple modules will automatically integrate to achieve composable reasoning. This approach then restricts interactions between modules in a way similar to how types do: a module’s tests must interact with the tests of other modules (via their usage as fakes), rather than directly depending on each other. Because all interaction between modules must occur via tests, the tests begin to feed off of each other, hopefully creating a virtuous cycle in the testing process. 

### François Pottier - Strong automated testing of OCaml libraries

This is about using an off-the-shelf fuzzer to perform unit testing of a library as a black box. This requires describing the specification (the API) of the library: I propose a set of combinators to do so. I do not yet have slides for this talk; I will probably have time to prepare just a few slides plus a demo. There is a paper: http://cambium.inria.fr/~fpottier/publis/pottier-monolith-2021.pdf
The slides are here: http://cambium.inria.fr/~fpottier/slides/fpottier-2021-06-monolith.pdf

### Matthias Hauswirth - A Notional Machine for Teaching Expressions

https://progmiscon.org (Programming Language Misconceptions)
Misconceptions related to concept "expression"
Misconceptions representable in "expression as tree" notional machine
https://expressiontutor.org (The tool I describe in this talk)

Humans consist mostly of water. Programs consist mostly of expressions. If our goal is to teach programming, we need to teach to read, write, and understand expressions. We developed a tool, Expression Tutor, to help teaching and assessing the conceptual understanding of expressions. The tool supports activities such as parsing, typing, evaluating, and unparsing expressions. It essentially repurposes the AST as a "notional machine" for "visual program simulation", where steps that compilers and program analyses tools do automatically have to be done manually by students who learn to program. To demonstrate that Expression Tutor can be used as a tool in teaching almost any language, we are currently creating brief example sequences of activities as they could be used to teach ideas such as method invocation in Java, list comprehensions in Python, spread syntax in JavaScript, desugaring in Scala, Boolean logic in Racket BSL, currying in Haskell, Church Booleans in lambda calculus, and even elementary algebra. I will briefly present the background, give a demo, and discuss limitations and open questions of our approach. I'd be more than happy to hear critical comments, feedback, and also potential interests in collaborations.

### John Hughes: Testing Smart Contracts with QuickCheck

We’ve recently developed an extension to QuickCheck for testing smart contracts in IOHK’s Plutus language. It’s based on state machine models, but includes a new feature inspired by dynamic logic for expressing and testing liveness properties. I can explain the context and the idea via a simple example of a Plutus smart contract.

### Tijs van der Storm: REPL-first language design

At Onward! last year I presented a paper on a principled approach to REPL interpreters. The paper looked at how the concept of a sequential language (“concatenating two programs is a program”) supports the design and implementation of REPL interpreters. In this talk I would like to broaden the perspective, to a kind of REPL-first language design, where the REPL is the leading “interface” to a programming language implementation. The commands typed in at the prompt can be framed as a very general and flexible linguistic “API” to the language, unifying user triggered UI events, program edit operations, state queries, and debugging commands. As such, the REPL can be used to manipulate both the program itself and the run-time state during its execution. The command history of the REPL thus subsumes (and interleaves) both versioning and execution history. I will demonstrate an experimental IDE for a DSL that illustrates the concept, featuring live programming, debugging, time-travel, and the usual REPL features.

###  Joe Politz: Pedagogic Issues with REPLs

REPLs are a common programming tool, and often used pedagogically. They allow for experimentation in live demonstrations, they juxtapose expressions with the values they produce, and they avoid a curricular dependency on printing to get interesting output.

REPLs also have significant UX weaknesses for early programming. This talk details some of these weaknesses that I've seen repeatedly while teaching many different audiences: the REPL introduces subtle state into the programming experience; learners are confused by what is editable and where the program lives; and REPL entries can have slightly different semantics than programs. These weaknesses are described with examples at https://jpolitz.github.io/notes/2020/07/10/repl-problems.html.

The talk presents alternate models and a prototype of a REPL-like programming environment for novices that addresses these issues, maintains many strengths, and opens up interesting future possibilities.

(I promise I wrote this before reading Tijs's abstract!)

### Jan-Willem Maessen: Accurate Type Analysis with BDDs

[Don’t schedule me for Wed; I may have to skip out of the session early.  Tues and Fri are optimal, Thu is fine.  Mon is currently cutting things a bit close.]

Our project at Facebook recently transitioned from a union/intersection/difference based type representation to one based on (Ordered) Binary Decision Diagrams.  The types we’re talking about here represent flow-sensitive runtime types, rather than the types that are checked by the type checker (in particular, our types are accurate: there’s no notion of back doors).  We’re interested in answering subtype and disjointness queries using flow-sensitive inference.  Because of the size of our programs we must handle millions of classes. A single inferred type can name thousands of individual classes.  Doing all this using unions and intersections is fairly straightforward and well-established.  Adding type difference makes things substantially more complicated – the combination of the subtyping and the law of the excluded middle resulted in a bug-ridden and hard-to-read wodge of code.  By switching to a BDD-based representation, we were able to dramatically simplify these algorithms.  However, we had to develop a reasonable type normalization algorithm: we want to know that if two types are equivalent, they’re equal.  In this talk, I’ll describe the normalization algorithm and some of the other challenges we’ve faced.

### Jonathan Aldrich: Gradual Verification

Current static verification techniques do not provide good support for incrementality, making it difficult for developers to focus on specifying and verifying the properties and components that are most important. Dynamic verification approaches support incrementality, but cannot provide static guarantees. To bridge this gap, we propose gradual verification, which supports incrementality by allowing every assertion to be complete, partial, or omitted, and provides sound verification that smoothly scales from dynamic to static checking. I’ll describe a system that can verify first-order specifications of programs that manipulate recursive, mutable data structures on the heap. Our approach addresses several technical challenges, such as semantically connecting iso- and equi-recursive interpretations of abstract predicates, and supporting gradual verification of heap ownership. This work thus lays the foundation for future tools that work on realistic programs and support verification within an engineering process in which cost-benefit trade-offs can be made.

(META: As usual, I have a lot of stuff going on...could also give an update on Penrose or Capabilities in Wyvern, talk about recent work on tweaking the DOT formalism to make it decidable, or talk about emerging work we’re doing on a language for time-sensitive sensor networks.  I proposed Gradual Verification as potentially the best combination of new/substantive/exciting, but if one of the other topics sounds better let me know.)

### James Noble: Computer Languages as Human Languages


It’s become a truism that “Programs must be written for people to read, and only incidentally for machines to execute” (Ableson & Sussman, first edition preface). If this is the case, then programming languages must first be designed for people to communicate with each other, and only then for computers, compilers, interpreters, and all the other paraphernalia of our discipline. In this talk I’ll explore some of the ways we can consider Computer Languages as Human Languages, and speculate on some of the advantages of doing so.

(META: this is preparation for part of a keynote talk, programmingLanguage as Language, that Robert BIddle and I are giving to HOPL IV)
