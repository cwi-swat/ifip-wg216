# Delft 2023

The (short) Delft 2023 meeting will be held at TU Delft, on 3rd and 4th of April, the two days
before the [Eelco Visser Commemorative Symposium](https://symposium.eelcovisser.org/) on 5th of April.

The meeting will be co-located with [IFIP WG 2.11 Program Generation](https://wiki.hh.se/wg211/index.php/Main_Page).

For general logistic information please consult the WG 2.11 pages [here](https://wiki.hh.se/wg211/index.php/WG211/M22Schedule).

## Talks



### Yannis Smaragdakis: Bug Patterns in Solidity Smart Contracts. Can Language Design Save the Day?

The Solidity language has emerged as the undisputed leader in smart contract development, for programmable blockchains. I will discuss a few bug patterns that have been behind real-world vulnerabilities (with some financial impact … like billions) and are based entirely on “surprising” semantics of language features.

Clearly, everyone in WG 2.16 will conclude from these examples that language design matters a lot for program correctness. … Yawn … So, I’ll play devil’s advocate and argue that it doesn’t. (Maybe because I believe it, maybe because it’s more interesting to argue.) I’ll show an example of what happens in practice in the Scilla language, which tries to preclude by-design reentrancy vulnerabilities. Just like God, if the devil didn’t exist, we’d have to invent him.

### Tom Van Cutsem: Exploring the design space of smart contract languages

Ilya Sergey’s paper “The Next 700 Smart Contract Languages” introduces a design space for languages to program smart contracts (programs executed by blockchain networks), with trade-offs between their safety and expressivity. I will discuss ongoing work by my students related to smart contract languages that touches on this trade-off. The first line of work is about a detailed comparison of Solidity (the leading smart contract language on Ethereum) with Move (the language used by emerging blockchains such as Aptos and Sui). The second line of work is about a study of dynamic access control patterns in Solidity, and how to refactor contracts to express these patterns using declarative constraint models. I welcome feedback and critique from the group to help shape the future directions of these explorations.

### Robby Findler: Esterel in Racket

Concurrency and thread preemption are tools that can make programs more modular. Unfortunately, in conventional programming models, combining state and concurrency (to say nothing of preemption!) makes programs extremely hard to reason about. Esterel offers a different programming model that is designed such that concurrency, state change, and thread preemption can all be used harmoniously. It dates to the 1980s and is the brainchild of Gérard Berry.

I have been working on a new implementation technique for Esterel that integrates more seamlessly with a conventional programming language. I'll try to use examples to make some sense out of what's written in the previous paragraph and, more generally, give a demo of this new implementation. If we have time, I'll try to explain how the implementation actually works and achieves this better form of integration.

### James Noble: Convergent Evolution

Everybody’s talking about Regions and Lifetimes, but it’s all Ownership to me

Rust has popularised ownership type systems that grant programmers explicit control or their programs’ memory management, within the context of a practical systems programming language. Rust’s design draws on more than 30 years of work across many different programming language research communities: linear functional programming (ICFP), region allocation (PLDI), ownership types (OOPSLA), alias burying (ECOOP).

This talk - based on a POPL 2023 tutorial curated jointly with Tobias Wrigstad - will attempt to argue that Rust’s lifetimes, ML’s regions, Pony’s capabilities, C++’s unique_ptr are examples of Convergent Evolution in programming language design.  Compressing six hours of material from a nominally three-hour tutorial into a 3 second “blipvert”, I’ll go on to speculate about likely further trajectories of language designs and ownership.



### François Pottier: An Ample-Step Semantics for (a fragment of) OCaml

This is not about language design per se, but I could give a talk about
ongoing work on the design and implementation of a formal semantics, inside
Coq, for a fragment of OCaml. This semantics is expressed in a style that is
a hybrid between two classic styles of semantics, namely (big-step) monadic
interpreters and (small-step) reduction semantics. Monadic interpreters are
attractive because they are easy to write and understand and they are
executable (inside Coq). Reduction semantics are attractive because they
support some side effects (such as divergence, non-determinism,
parallelism, concurrency) more easily. So far, the semantics supports a
small fragment of OCaml and I have constructed a sound Hoare logic for it.
Future work includes growing this language fragment and scaling up from
Hoare logic to a modern separation logic (namely, Iris).

### Klaus Ostermann:  The Proof Expression Problem


### Jan-Willem Maessen: Diff Sketching: Poor Man’s Language-Independent Diff-Time Program Analysis

Unintentional errors in API use can result in privacy incidents.  We’d like to catch these problems at code review time, before code reaches production.  From a classical program analysis perspective, this is a solved problem – taint analysis lets us track flows of private data from sources to sinks and flag the flows that look suspicious.  But: Our code base was hundreds of millions of lines in numerous languages in 2019 and has grown steadily since then.  Many of these languages lack fast-turnaround static analysis tools (especially given the size of our code base), and essentially none uniquely identify calls that act as sources and sinks: data APIs are rarely written in a way that cleanly separates sensitive and non-sensitive data.  Meanwhile, if we want to catch potential problems at diff time, we should flag newly-created incomplete flows (flows from a source into a diff’s code, or from a diff’s code into a sink).  So what looks like a taint analysis problem is nothing of the sort!  Instead, we are building a suite of API-specific detectors around a diff sketch.  This is a high-level language-independent summary of code changes in the diff.  We pair this with Glean, which contains a full index of our source code at a recent stable commit.

### Tobias Wrigstad: Deferred Evacuation

I will talk about the a tension between marking and evacuation in concurrent GC.
An efficient way to free memory in garbage collection is to evacuate a page (a memory space) leaving all dead objects to be overwritten by subsequent allocation. On a completely full page, evacuation is just a waste of CPU since no memory can be reclaimed because of it. Therefore, a typical approach is to evacuate only sparsely populated pages which gives maximal ”return on investment”: copy few objects, get whole page in return. Detecting that a page is sparse requires information about liveness that takes time to compute as it requires traversing the entire heap. Due to this delay, liveness and density information may be incorrect by the time it is used to drive evacuation. This may lead to extraneous copying of objects which is wasteful of both memory and CPU. I will talk about this tension, and how we try to use it to our favour by defining a GC algorithm that gets away with doing less work, but delaying evacuation even further.

### Jonathan Aldrich: Initial Implementation and Experience with Gradual Verification

Current static verification techniques do not provide good support for incrementality, making it difficult for developers to focus on specifying and verifying the properties and components that are most important. Dynamic verification approaches support incrementality, but cannot provide static guarantees. To bridge this gap, we proposed gradual verification, which supports incrementality by allowing every assertion to be complete, partial, or omitted, and provides sound verification that smoothly scales from dynamic to static checking. I’ll describe a system that can verify first-order specifications of programs that manipulate recursive, mutable data structures on the heap, demonstrate a prototype tool, and share some initial empirical results. Since this is a language design workshop, I’ll highlight some aspects of specification design that are important for making gradual verification practical. We hope this work lays the foundation for future tools that better support verification within an engineering process in which cost-benefit tradeoffs can be made.

### Martin Odersky: Back to Direct Style with Capabilities

Effect typing has seen increasing industrial adoption, mostly driven by async, reactive programming, and other concurrency patterns. But it is far from being a clear success. For instance, most approaches suffer from the so-called colored function problem which is due to a lack of effect polymorphism. Combining different effect types is also generally hard. No wonder then, that most effect typing systems are seen as annoyingly brittle and complex. This holds for checked exceptions in Java, as well as for async functions in Rust, or monadic effects systems like cats effect in Scala. 

Can we do better? It turns out that we can get effect polymorphism and flexible composition if we shift our viewpoint from (monadic) effects to object capabilities. To keep type safety, these capabilities need to be tracked in types. This is the approach we explore in Caprese. We model captured capabilities in an experimental Scala extension. Combined with delimited continuations, this allows the formulation of safe direct-style control effects which promise much improved composability and flexibility.

### Andreas Rossberg: Engineering a Language Specification

Wasm is an industrial-strength language technology whose standard includes a complete formal specification, which has been machine-verified. It is also evolving quite substantially. Evolving such a language and its specification poses a number of challenges and is rather laborious. I will present our new experiment for simplifying this procedure, which involves a DSL for authoring and generating significant parts of the specification as well as feeding into other consumers.


### ~~Tijs van der StormRegelspraak vs the Questionnaire Language (QL): same same but different?~~

~~Regelspraak (“Rulespeak”) is a controlled natural language (CNL) used, among others, by the Dutch tax authority to define various tax rules and regulations. QL is a small DSL for defining interactive questionnaires, initially designed as a benchmark language to compare language workbenches. While both languages were invented independently, it turns out there are some striking similarities between the two, and the differences turn out to be more superficial than you’d initially think. In this talk I’ll discuss both languages, and how they cover in some way the same ground but from different directions and stakeholder viewpoints. Both languages can be interpreted in complementary ways, which sheds new light on how checking of rules and (conditional) gathering of information can be seen as two sides of the same coin.~~

### Tijs van der Storm: Salix: Elm-style Web programming in Rascal, an exercise in library design

Elm is small purely functional language for web-programming designed by Evan Czaplicki. I’ve ported this language to Rascal as an embedded DSL/library. I will discuss some trade-offs and challenges in the design and demonstrate its abilities and limitations. 
