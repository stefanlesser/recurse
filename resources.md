# Study Resources
_My big dumping ground for links to articles, (e)books, videos and similar material that caught my attention, but I haven't had the time to look at yet. I'm still figuring out how to work with this list…_

Resources marked with ★ are recommended starting points or must read|watch material for the given category.

----

## Dive into advanced functional programming concepts with Haskell and Swift

### Start Here
These are my recommended resources to start with, if you are planning to go down the same path and learn functional progamming.

* [x] [★ Functional Programming Basics - What’s It All About?](https://pragprog.com/magazines/2013-01/functional-programming-basics)
    <br>"Functional Programming is progamming without assignment statements." This means data in memory is (mostly) immutable and that makes parallelism for multiple CPU cores much easier to reason about. This article is a very high-level introduction into one of the core concepts of FP and ties it to one of the main benefits. I do think there's more to it than that, but this should get you excited about it.
* [x] [★ 📺 (30m) Functional programming patterns for the non-mathematician (cut)](https://www.youtube.com/watch?v=AvgwKjTPMmM)
    <br>Good introduction on how you can practically use composition, lenses, (which are built on monoids, functors, applicatives, and monads) for nesting (composition), null checking (Maybe), error handling (Either), and accumulation (reduce) in JavaScript.
* [x] [★ Getting started with Haskell • Stack Overflow](https://stackoverflow.com/questions/1012573/getting-started-with-haskell/1016986#1016986)
    <br>Gives you a high-level overview of what the journey of learning Haskell can look like. Several good pointers to articles and resources.
* [x] [★ 📕 PureScript by Example](https://leanpub.com/purescript/read)
    <br>PureScript's syntax and libraries are almost identical to Haskell's, and this book is much shorter and more practical. I'd recommend learning PureScript (and Haskell) by starting with this book.
* [x] [★ 📕 Haskell Programming from First Principles](http://haskellbook.com)
    <br>Massive introduction into Haskell with lots of explanation and exercises. Some people find it too exhaustive, but I like this book much better than the free "Learn you a Haskell", although it's still very academic. It starts off with a very abstract introduction to lambda calculus, which I believe is an important basis to know about before diving into Haskell. It does make the first chapter a little strange — keep reading and don't judge the book until after chapter 2.
* [x] [★ Monoids, Functors, Applicatives, and Monads: 10 Main Ideas](https://monadmadness.wordpress.com/2015/01/02/monoids-functors-applicatives-and-monads-10-main-ideas/)
    <br>Great summary of the key points on the four algebras that show up everywhere in Haskell (and are hiding in other languages as well).
* [ ] [★ Haskell Typeclassopedia](https://wiki.haskell.org/Typeclassopedia)
    <br>Given how important it is to understand types in Haskell, this article explains the most abstract (read: used everywhere) type classes in great detail and helps form an intuitive understanding of functor, applicative, and monad.
* [ ] [★ Diehl: What I Wish I Knew While Learning Haskell](http://dev.stephendiehl.com/hask/)
    <br>The first two secions *Basics* and *Monads* are packed with great practical tips and a solid foundation for understanding monads, an abstract concept that shows up everywhere in Haskell and functional programming.

### General
* [x] [The Unofficial Guide to Rich Hickey's Brain](http://www.flyingmachinestudios.com/programming/the-unofficial-guide-to-rich-hickeys-brain/)
    <br>Contrasts Object-Oriented Programming with Functional Programming and explains the "fundamental flaws' of accidential complexity in OOP that FP allows us to deal with in a better way.
* [x] [📺 (60m) "I See What You Mean" by Peter Alvaro](https://www.youtube.com/watch?v=R2Aa4PivG0g)
    <br>Entertaining presentation about modeling state with declarative languages. Many applicable concepts although it is understandably a little heavy on the relational language this talk is about.
* [x] [From Higher-Order Functions to Libraries And Frameworks](http://raganwald.com/2016/12/15/what-higher-order-functions-can-teach-us-about-libraries-and-frameworks.html)
    <br>How higher-order functions influence the expressiveness and complexity of programs. This is part 1 of a series of 3 articles.
* [x] [Functional Programming is taking over UIs with Pure Views](https://medium.freecodecamp.com/the-revolution-of-pure-views-aed339db7da4)
    <br>Why functional programming helps keeping the user interface layer simple and enables hot module replacement, time-travel debugging and similar features.
* [x] [A Beginner-Friendly Tour through Functional Programming in Scala](http://degoes.net/articles/easy-monads)
    <br>Introduces benefits of functional programming by transforming a simple console program from imperative to declarative step by step. Even though it's using Scala, it helps understanding the basic building blocks of FP and their benefits.
* [x] [Destroy All Ifs — A Perspective from Functional Programming](http://degoes.net/articles/destroy-all-ifs)
    <br>By replacing conditionals with lambdas, we can invert control and make our code both easier to reason about and more generic. Moving conditionals from places hidden in the deepest nested function up to the caller makes intent clear and prevents mistakes.
* [ ] [Functional Programming with Bananas, Lenses, Envelopes and Barbed Wire](http://eprints.eemcs.utwente.nl/7281/01/db-utwente-40501F46.pdf)
* [ ] [Streaming Combinators and Extracting Flat Parallelism](http://futhark-lang.org/blog/2017-06-25-futhark-at-pldi.html)
* [ ] ? 📕 Modeling Data with Functional Programming in R

### Haskell
* [x] [Learn Haskell the hard way](http://yannesposito.com/Scratch/en/blog/Haskell-the-Hard-Way)
    <br>Just as promised in the title, an introduction to Haskell from zero to monads in a rather short article. I don't think this is a good tutorial to start with, but after reading about the concepts in other places, the additional examples and different ways of explaining monads in this article are very helpful.
* [x] [💡 Scalable program architectures](http://www.haskellforall.com/2014/04/scalable-program-architectures.html)
    <br>Explains the core concept of composition with monoids: combine several components together of type A to generate a new component of the same type A, indistinguishable in character from its substituent parts. These abstractions scale limitlessly because they always preserve combinability, therefore we never need to layer further abstractions on top.
* [x] [💡 The category design pattern](http://www.haskellforall.com/2012/08/the-category-design-pattern.html)
* [x] [💡 The functor design pattern](http://www.haskellforall.com/2012/09/the-functor-design-pattern.html)
    <br>Functors are adapters that bridge between categories. Instead of rewriting functions for a different category, a functor allows you to re-use the existing function to work in another category.
* [x] [Queer Types - Applicatives and Alternatives](https://queertypes.com/posts/59-applicatives-alternatives.html)
    <br>Practical introduction into how applicatives (and alternatives, which build on it) can be used.
* [x] [Foldable and Traversable](https://blog.jakuba.net/2014/07/30/foldable-and-traversable.html)
* [x] [Haskell/Understanding monads/State](https://en.wikibooks.org/wiki/Haskell/Understanding_monads/State)
* [x] [Scalable program architectures](http://www.haskellforall.com/2014/04/scalable-program-architectures.html)
* [x] [Equational reasoning at scale](http://www.haskellforall.com/2014/07/equational-reasoning-at-scale.html)
* [x] [📺 (1h:30m) C++Now 2017: Ryan Newton "Haskell taketh away: limiting side effects for parallel programming"](https://www.youtube.com/watch?v=lC5UWG5N8oY)
    <br>Fascinating look into the direction and development of Haskell.
* [ ] [📺 Tangible Functional Programming](http://youtube.com/)
* [ ] [📺 (60m) Fastware - Andrei Alexandrescu](https://www.youtube.com/watch?v=o4-CwDo2zpg)
* [ ] ? [EdX course: Introduction to Functional Programming (via Haskell)](https://www.edx.org/course/introduction-functional-programming-delftx-fp101x-0)
* [ ] ? [Haskell Communities and Activities Report • 32nd Ed. May 2017](https://www.haskell.org/communities/05-2017/html/report.html)

#### Practical Haskell
* [x] [📕 Purely Functional Data Structures](https://www.cs.cmu.edu/~rwh/theses/okasaki.pdf)
    <br>Proves that purely functional data structures can be as fast as imperative algorithms thanks to memoization and clever algorithm design.
* [ ] [📕 Real World Haskell • Bryan O'Sullivan, Don Stewart, and John Goerzen](http://book.realworldhaskell.org/read/)
    <br>This book promises to teach more practical Haskell, which makes it a welcome alternative to all the academic books out there. *Haven't read it yet, so I don't know if that's true.*
* [ ] [📕 Parallel and Concurrent Programming in Haskell](http://chimera.labs.oreilly.com/books/1230000000929/index.html)
    <br>This book get mentioned and referred to a lot, surprisingly not just for topics around the book's title.
* [x] [The Fun of Programming • Ch. 7 Functional Images](http://conal.net/papers/functional-images/fop-conal.pdf)
    <br>Creating visual patterns with math based on transformation functions. Great example of how composing small components can yield complex effects.
* [ ] [📺 (45m) Manuel Chakravarty - Haskell SpriteKit: A Case Study in Turning a Stateful into a Functional API](https://www.youtube.com/watch?v=H_z4NKvxf1U&app=desktop)
* [ ] [Introduction to brick, a Haskell library for building terminal user interfaces](https://samtay.github.io/articles/brick.html)
* [x] [Writing Video Games in a Functional Style](http://prog21.dadgum.com/228.html)
    <br>A collection of articles exploring the implementation of arcade games and their game state and game loops in a functional style.
* [x] [Code Us Some Roguelike in Haskell (Part 2)](http://jamiltron.com/2012/07/Code_Us_Some_Roguelike2.html)

#### Haskell Resources
* [Haskell Wiki](https://wiki.haskell.org/)
* [Hoogle](https://www.haskell.org/hoogle/) — Enter a type signature and it will find you matching functions
* [Hayoo](http://hayoo.fh-wedel.de/) — Same but with support for third-party packages
* [Vim and Haskell in 2016](http://www.stephendiehl.com/posts/vim_2016.html) — How to set up your dev env with vim for Haskell

### PureScript
* [x] [📺 Luka Jacobowitz - Reactive Programming in the Browser with Scala.js and PureScript](https://m.youtube.com/watch?v=pE-3bg31Jlo)
* [x] [📺 Intro to PureScript - Utah Haskell Meetup](https://m.youtube.com/watch?v=9a57V3bvzaI)
* [x] [📺 PureScript & Pux ~ Front End Authority (Oct 2016)](https://youtu.be/NmT5-j3-xzg)
* [x] [Pux](http://purescript-pux.org)

### Swift
* [x] [📺 (45m) Brandon Williams - Finding Happiness in Functional Programming](https://www.youtube.com/watch?v=A0VaIKK2ijM)
    <br>Exploring the benefits and downsides of functional conepts in practical use, from isolation of side (and co-)effects to coding for an interface we wish we had instead of the one we're given. Great points about how to encapsulate state management with lenses using UIKit as an example.
* [x] [📺 (10 Talks) Functional Swift Conference 2017](http://2017.funswiftconf.com)
* [x] [💡 📺 (25m) Brandon Kase: Composable Caching in Swift](https://www.youtube.com/watch?v=8uqXuEZLyUU)
    <br>Using a monoidal structure to simplify layered caching with composable caches.
* [x] [💡 📺 (40m) Brandon Kase: Beyond Types in Swift](https://m.youtube.com/watch?v=6z9QjDUKkCs)
    <br>Adding functionality without adding complexity through abstract algebra:
    - Magma: closed binary operators = composable operation
    - Semi-group: + associativity = parallelization
    - Monoid: + identity = dropping the optional
    - Commutative Monoid: + commutativity = reorder
    - Bounded Semilattice: + idempotence = no need for memory
* [x] [💡 📺 (40m) Monoids, Predicates and Sorting Functions](https://www.youtube.com/watch?v=VFPhPOnPiTY)
    <br>This demonstrates the practical application of the other Brandon's talk above with live coding in Swift Playgrgounds. Impressive composability of the simplest components by building them up following the rules and laws.
* [x] [Swift Enums Are "sum" Types. That Makes Them Very Interesting](https://mislavjavor.github.io/2017-04-19/Swift-enums-are-sum-types.-That-makes-them-very-interesting/)
    <br>Explains product and sum types and shows how they can be used to minimize possible use cases and define away potential error states. With examples for use cases for sum types (enums) like router and theme patterns and tree data structures.
* [x] [Algebraic Structure and Protocols](http://www.fewbutripe.com/swift/math/algebra/2015/02/17/algebraic-structure-and-protocols.html)
    <br>This article takes a mathematical approach to introduce monads through semigroups.
* [x] [The Algebra of Predicates and Sorting Functions](http://www.fewbutripe.com/swift/math/algebra/monoid/2017/04/18/algbera-of-predicates-and-sorting-functions.html)
    <br>Extends the knowledge about semigroups and monoids to introduce predicate and sorting functions.
* [x] [📺 (30m) Brandon Williams - Lenses in Swift](https://www.youtube.com/watch?v=ofjehH9f-CU)
    <br>Using lenses and prisms to create getters and setters for immutable values.
* [x] [An aside about flatMap and monads](https://www.cocoawithlove.com/blog/an-aside-about-flatmap-and-monads.html)
    <br>Practical notes on Monads in Swift and Haskell, and how Swift's flatMap sometimes is a proper monad and sometimes isnt't (and why that's totally fine).
* [x] [Composable HTML Views in Swift](http://www.fewbutripe.com/swift/html/dsl/2017/06/29/composable-html-views-in-swift.html)
    <br>Improving an eDSL for generating HTML in Swift with the powers of abstract algebra in form of Monoids.
* [ ] [Loose coupling using default implementations in protocol extensions](http://www.apokrupto.com/blog-1/2017/5/16/default-protocol-extensions-for-loose-coupling)
* [ ] [Data Sources in Swift… or how to avoid that this new trendy persistence framework determines the architecture of your App](https://medium.com/@dcordero/data-sources-in-swift-or-how-to-avoid-that-this-new-trendy-persistency-framework-determines-the-5472fcb75eda)
* [ ] [📺 (20m) Optimizing Swift Collections • Károly Lőrentey at dotSwift 2017](https://www.dotconferences.com/2017/01/karoly-lorentey-optimizing-swift-collections)
    <br>Deep dive into performance characteristics of Swift Collection types.
* [ ] [Apple Swift Ownership Manifesto](https://github.com/apple/swift/blob/master/docs/OwnershipManifesto.md)
* [ ] [The Elm Architecture in Swift](https://github.com/chriseidhof/tea-in-swift)

#### Practical Swift
* [ ] [Highlights from Realm Live at WWDC and AltConf](https://news.realm.io/news/realm-live-at-wwdc-and-altconf/)
* [ ] [iOS Simulator Power Ups](https://medium.com/the-traveled-ios-developers-guide/ios-simulator-power-ups-407060863b3c)
* [ ] [Swift 4 Decodable: Beyond The Basics](https://medium.com/swiftly-swift/swift-4-decodable-beyond-the-basics-990cc48b7375)
* [ ] [JSON with Encoder and Encodable](https://swiftunboxed.com/stdlib/json-encoder-encodable/)
* [ ] [Swift — memoize() walk through](https://medium.com/@mvxlr/swift-memoize-walk-through-c5224a558194)
* [ ] [Functional Swift and Memoization](http://blog.scottlogic.com/2014/09/22/swift-memoization.html)
* [ ] [How we cut our iOS app’s launch time in half](https://blog.automatic.com/how-we-cut-our-ios-apps-launch-time-in-half-with-this-one-cool-trick-7aca2011e2ea)
* [ ] [📺 (25m) Dealing With Asynchrony in a Synchronous Swift World](https://news.realm.io/news/greg-heo-dealing-asynchrous-synchronous-swift-swift-language-user-group-2017/)
* [ ] [📺 Writing Your UI Swiftly](https://news.realm.io/news/sommer-panage-writing-your-ui-swiftly/)
* [ ] [My Development Toolset 2017 for iOS](https://medium.com/ios-os-x-development/my-development-toolset-2017-for-ios-7c0758e3e5ce)

### Category Theory
* [x] [Haskell/Category theory](https://en.wikibooks.org/wiki/Haskell/Category_theory)
    <br>After being familiar with using functors, monoids, and monads in Haskell, this article introduces just enough category theory to understand the maths behind those concepts.
* [x] [📺 (60m) Category Theory for the Working Hacker by Philip Wadler](https://www.youtube.com/watch?v=V10hzjgoklA)
    <br>If you want to take it an abstraction level higher, this surprisingly entertaining talk explains the math behind lambda calculus called category theory.
* [x] [Monads Made Difficult](http://www.stephendiehl.com/posts/monads.html)
    <br>Explains monads coming from category theory. This is only helpful if you enjoy the math a lot.
* [x] [Duality for Haskellers](http://blog.ezyang.com/2012/10/duality-for-haskellers/)
    <br>Explains the concept of duality in category theory using sum/product, top/bottom, and fold/unfold on lists.
* [x] [Flipping arrows in coBurger King](http://blog.ezyang.com/2010/07/flipping-arrows-in-coburger-king/)
    <br>Explains co-monad and duality and the concept of "flipping arrows" in category theory.
* [x] [Data and Codata](http://blog.sigfpe.com/2007/07/data-and-codata.html)

### Functional Patterns to Manage Complexity
* [x] [💡 The future of software, the end of apps, and why UX designers should care about type theory](https://pchiusano.github.io/2013-05-22/future-of-software.html)
    <br>Paints an interesting picture of a world where composing components is much simpler and instead of apps that have been put together by developers, regular users are able to compose service components to do what they want them to do.
* [x] [💡 📺 (60m) Gabriel Gonzales: Applied category theory and abstract algebra - λC Winter Retreat 2017](https://www.youtube.com/watch?v=WsA7GtUQeB8)
    <br>"[We can] tackle software complexity by reusing standard interfaces that originate in the fields of category theory and abstract algebra." Builds understanding for composition going from composable functions to composable values (monoids) to composable types (applicatives) and shows how powerful these concepts are to decompose programs into simple building blocks.
* [x] [💡 A Modern Architecture for FP](http://degoes.net/articles/modern-fp)
    <br>"We shouldn’t write programs — we should write descriptions of programs, which we can then introspect, transform, and interpret at will." How to architect a program that uses separate layers of DSLs to encode business logic in separate domains, and having an interpreter combining those DSLs to generate the actual program. It seems cumbersome to do this, but the composability of this approach looks promising.
* [x] [💡 Modern Functional Programming: Part 2](http://degoes.net/articles/modern-fp-part-2)
    <br>John edited his thoughts in part 1 into a more coherent and clear picture in this article and gives a glimpse into the future of programming by combining interpreters for different DSLs.
* [x] [📺 (45m) Sandy Maguire: Don't Eff It Up: Free Monads in Action](https://www.youtube.com/watch?v=gUPuWHAt6SA)
    <br>Shows a technique to combine different side effects with free monads using the Eff(ects) monad, which can be used as an alternative to monad transformers with less boilerplate.
* [x] [📺 (40m) John A De Goes: MTL Versus Free Deathmatch - λC 2016](https://www.youtube.com/watch?v=JLevNswzYh8)
    <br>Fun talk diving deeper into John's thoughts about the future of programming with abstract functional structures generating and manipulating the program before it's being executed.
* [x] [📺 (1h:15m) John DeGoes: Beyond Free Monads - λC Winter Retreat 2017](https://www.youtube.com/watch?v=A-lmrvsUi2Y)
    <br>More thoughts about John's vision of programming with absctract functional concepts and why we need a better programming language to actually make that future happen.

----

## Build interpreter/compiler and create simple programming language from scratch
* [x] [Rich Programmer Food](http://steve-yegge.blogspot.com/2007/06/rich-programmer-food.html?m=1)
* [x] [So You Want To Write Your Own Language?](http://www.drdobbs.com/architecture-and-design/so-you-want-to-write-your-own-language/240165488)
    - Focus on: context-free grammar, good diagostics (redundancy helps), tried and true grammatical forms for familiar constructs. Ignore: minimizing keystrokes, easy parsing, minimizing keywords, lexer or parser generators.
    - Use a poisoning approach for marking errors in the AST, like in D.
    - Use a profiler to find performance issues.
    - Take advantage of lowering (rewriting more complex semantic constructs in terms of simpler ones, e.g. while and for-each loops can both be rewritten as for loops).
    - Don't forget that a good runtime library is important. Don't have too much trivia in it.
* [x] [Building a Primitive State Machine in Haskell](https://daniel-levin.github.io/2015/01/19/primitive-state-machine-in-haskell.html)
    <br>Brief article with a very simple state machine implmented in Haskell using pattern matching.
* [ ] [Turing Machines and Tooling, Part I](http://raganwald.com/2017/04/06/turing-machines.html)
* [ ] [Turing Machines and Tooling, Part II](http://raganwald.com/2017/04/16/turing-machines-part-ii.html)
* [x] [Write Yourself a Scheme in 48 Hours](https://en.wikibooks.org/wiki/Write_Yourself_a_Scheme_in_48_Hours)
    <br>With basic Haskell knowledge this course is quick and easy to get into, but it also doesn't explain concepts very extensively.
* [ ] [Building a LISP from scratch with Swift](https://www.uraimo.com/2017/02/05/building-a-lisp-from-scratch-with-swift/)
* [ ] [A simple LISP interpreter written in Swift](https://github.com/hollance/BuildYourOwnLispInSwift)
* [ ] [Implementing a JIT Compiled Language with Haskell and LLVM](http://www.stephendiehl.com/llvm/)
* [ ] ? [📕 Crafting Interpreters - A handbook for making programming languages • Bob Nystrom](http://www.craftinginterpreters.com)
    <br>Promising book currently in development. This might become the most approachable guide to writing interpreters and compilers. Unfortunately, it's not even halfway done yet.
* [ ] ? [Write Yourself Haskell](http://dev.stephendiehl.com/fun/)
* [ ] ? [Dragon taming with Tailbiter, a bytecode compiler for Python • codewords.recurse.com](https://codewords.recurse.com/issues/seven/dragon-taming-with-tailbiter-a-bytecode-compiler)

### Lambda Calculus
* [x] [The Lambda Calculus for Absolute Dummies (like myself) • palmström](http://palmstroem.blogspot.jp/2012/05/lambda-calculus-for-absolute-dummies.html)
    <br>Another lambda calculus tutorial.
* [x] [COMPUTATION STARTING FROM FIRST PRINCIPLES (DRAFT) • Jan Wedekind](http://www.wedesoft.de/binary-lambda-calculus.html)
    <br>Implementing a minimal language based on lambda calculus in C.
* [ ] [Data is Code](http://www.haskellforall.com/2016/04/data-is-code.html?m=1)
* [ ] [7 lines of code, 3 minutes: Implement a programming language from scratch](http://matt.might.net/articles/implementing-a-programming-language/)
* [ ] [Closure conversion: How to compile lambda](http://matt.might.net/articles/closure-conversion/)
* [ ] [Compiling to lambda-calculus: Turtles all the way down](http://matt.might.net/articles/compiling-up-to-lambda-calculus/)
* [ ] [Equational derivations of the Y combinator and Church encodings in Python](http://matt.might.net/articles/python-church-y-combinator/)
* [ ] [Fixed-point combinators in JavaScript: Memoizing recursive functions](http://matt.might.net/articles/implementation-of-recursive-fixed-point-y-combinator-in-javascript-for-memoization/)
* [ ] [The Y Combinator (Slight Return) or How to Succeed at Recursion Without Really Recursing](http://mvanier.livejournal.com/2897.html)

### Background
* [x] [Software structure for programmers who know at least one programming language](https://www.destroyallsoftware.com/compendium/software-structure/6fb5f711cae5a4e6)
* [x] [Types for anyone who knows a programming language](https://www.destroyallsoftware.com/compendium/types/baf6b67369843fa2)
    - Introduction to and overview of several different type systems in popular programming languages.
* [ ] [The memory models that underlie programming languages • canonical.org](http://canonical.org/~kragen/memory-models/)
* [ ] [Monadic Parsers: Implementing a micro Parsec](http://olenhad.me/articles/monadic-parsers/)
* [ ] [Swift Talk #13 Parsing Techniques](https://talk.objc.io/episodes/S01E13-parsing-techniques)
* [ ] [Parsing context-sensitive languages with Applicative](https://byorgey.wordpress.com/2012/01/05/parsing-context-sensitive-languages-with-applicative/)
* [ ] [📺 (45m) Modelica: Component Oriented Modeling of Physical Systems" by Michael Tiller](https://www.youtube.com/watch?v=-mvEUuc-sWE)
* [ ] [📺 (45m) Ceptre: A Language for Modeling Generative Interactive Systems" by Chris Martens](https://www.youtube.com/watch?v=bFeJZRdhKcI)
* [x] [A Tutorial Explaining LALR(1) Parsing](https://web.cs.dal.ca/~sjackson/lalr1.html)
    <br>Detailed walk-through of how to implement a parser based on a bottom-up approach.
* [x] [Earley Parsing Explained](http://loup-vaillant.fr/tutorials/earley-parsing/)
    - In-depth walk-through of how Early parsing works. Code samples in Lua.
* [ ] [Bounded Seas — Island Parsing Without Shipwrecks](http://scg.unibe.ch/archive/papers/Kurs14b-BoundedSeas.pdf)
* [ ] 📕 Concepts, Techniques, and Models of Computer Programming

Resources
* [Earley parser implementation • GitHub](https://github.com/lagodiuk/earley-parser-js)
* [FParsec Documentation](http://www.quanttec.com/fparsec/)

----

## Try (functional) reactive programming with RxSwift and/or React.js
* [x] [📺 (25m) Everyday Reactive](https://news.realm.io/news/everyday-reactive/)
    <br>Quick introduction to reactive programming with pros and cons and pointers to frameworks and resources.
* [x] [📺 (35m) Justin Spahr-Summers • Enemy of the State](https://m.youtube.com/watch?v=7AqXBuJOJkY)
    <br>Several arguments on why to minimize state and how to achieve that in Swift.
* [x] [Read A Farewell to FRP](http://elm-lang.org/blog/farewell-to-frp)
    <br>How elm is removing (hiding) the functional reactive programming patterns like streams, because they don't have to be exposed to create robust web apps.
* [x] [Josh Abernathy • Better Code for a Better World](https://speakerdeck.com/joshaber/better-code-for-a-better-world)
* [ ] [What is reactive programming and why should I use it?](https://www.cocoawithlove.com/blog/reactive-programming-what-and-why.html)
* [ ] [The introduction to Reactive Programming you've been missing](https://gist.github.com/staltz/868e7e9bc2a7b8c1f754)
* [ ] [Reactive programming from scratch](http://www.thomasvisser.me/2016/11/28/reactive-from-scratch/)
* [ ] [Do-It-Yourself Functional Reactive Programming](https://speakerdeck.com/mchakravarty/do-it-yourself-functional-reactive-programming)

Frameworks
* [Bond](https://github.com/ReactiveKit/Bond)
* [RxSwift](https://github.com/ReactiveX/RxSwift)
* [ReactiveCocoa](https://github.com/ReactiveCocoa/ReactiveCocoa)
* [CwlSignal](https://github.com/mattgallagher/CwlSignal)
* [Cycle.js](https://cycle.js.org)
* [elm — A delightful language for reliable webapps](http://elm-lang.org)

----

## Brush up my knowledge about (graph) data structures and algorithms
* TODO: add resources from reading list and iBooks

### Conflict-Free Replicated Data Types (CRDT)
* [ ] [Conflict-free replicated data type](https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type)
* [ ] [A Look at Conflict-Free Replicated Data Types (CRDT)](https://medium.com/@istanbul_techie/a-look-at-conflict-free-replicated-data-types-crdt-221a5f629e7e)
* [ ] [Conflict-free replicated data types](https://medium.com/@qt/a-brief-history-of-replicated-data-ab9dcf1671a0)
* [ ] [Conflict-free Replicated Data Types](http://muratbuffalo.blogspot.com/2013/04/conflict-free-replicated-data-types.html)
* [ ] [A comprehensive study of Convergent and Commutative Replicated Data Types](http://hal.upmc.fr/file/index/docid/555588/filename/techreport.pdf)
* [Readings in conflict-free replicated data types](http://christophermeiklejohn.com/crdt/2014/07/22/readings-in-crdts.html)

----

## Get back into JavaScript (and possibly TypeScript) and see what’s state of the art for web development (looking at React, Relay, GraphQL, Jest, etc.)
* [ ] [📕 You Don't Know JS (book series)](https://github.com/getify/You-Dont-Know-JS)
* [x] [Overview of ECMAScript 6 features](https://github.com/lukehoban/es6features)
* [x] [A Functional Programmer’s Introduction to JavaScript (Composing Software)](https://medium.com/javascript-scene/a-functional-programmers-introduction-to-javascript-composing-software-d670d14ede30)
* [ ] [http://jrsinclair.com/articles/2017/javascript-without-loops/index.html](http://jrsinclair.com/articles/2017/javascript-without-loops/index.html)
* [ ] [Higher Order Functions (Composing Software)](https://medium.com/javascript-scene/higher-order-functions-composing-software-5365cf2cbe99)
* [ ] [You Might Not Need Redux](https://medium.com/@dan_abramov/you-might-not-need-redux-be46360cf367)
* [ ] [Vue.js • Comparison with Other Frameworks](https://vuejs.org/v2/guide/comparison.html)
* [ ] 📕 Eloquent JavaScript

Reference
* [📕 Exploring ES6](http://exploringjs.com/es6/index.html)
* [Design Patterns in ES6](http://tcorral.github.io/Design-Patterns-in-Javascript/)
* [📕 Speaking JavaScript (ES5)](http://speakingjs.com/es5/index.html)

----

## Explore data visualization, procedural generation, and generative art — try d3.[js|express] and graphics programming with Metal or Vulcan

### Information Visualization
General
* [ ] [Information Visualization • Enrico Bertini](http://enrico.bertini.io/teaching/)
* [ ] [The death of interactive infographics?](https://medium.com/@dominikus/the-end-of-interactive-visualizations-52c585dcafcb)
* [ ] [📺 (60m) Dean's Lecture: The Past and Future of Data Analysis](https://www.youtube.com/watch?v=qFtJaq4TlqE)
* [ ] [The Gamma: Tools for open data-driven storytelling](https://thegamma.net)
* [x] [The seven deadly sins of statistical misinterpretation, and how to avoid them](http://theconversation.com/the-seven-deadly-sins-of-statistical-misinterpretation-and-how-to-avoid-them-74306)
* [ ] 📕 Thinking with Data
* [ ] [📕 The Grammar of Graphics](https://www.cs.uic.edu/~wilkinson/TheGrammarOfGraphics/GOG.html)

d3
* [ ] 📕 Interactive Data Visualization for the Web
* (alternative book option) 📕 [D3.js in Action, Second Edition](https://www.manning.com/books/d3js-in-action-second-edition)
* [x] [The Hitchhiker’s Guide to d3.js](https://medium.com/@enjalot/the-hitchhikers-guide-to-d3-js-a8552174733a)
    - Great starting point linking to many tutorials and resources to learn d3.js and it's underlying technologies (canvas, SVG). Most other resources in this list came from here.
* [x] [How do you learn d3.js?](https://medium.com/@enjalot/how-do-you-learn-d3-js-ccffc151419b)
    - Pick a project you want to do and then figure out how to do it. Let your motivation drive the choice of tools, instead of the other way around.
* [x] [Three Little Circles](https://bost.ocks.org/mike/circles/)
    - Introduction to binding data, enter and exit patterns.
* [x] [Thinking with Joins](https://bost.ocks.org/mike/join/)
    - Understanding data joins.
* [x] [General Update Pattern](https://bl.ocks.org/mbostock/3808218)
    - Three examples highlighting the update pattern and key functions (+ transitions).
* [x] [Introducing d3-scale](https://medium.com/@mbostock/introducing-d3-scale-61980c51545f)
    - Scales are the powerful concept of mapping a dimension of data to a visual representation. Or mapping an input domain to an output range.
* [x] [Interactive Data Visualization for the Web • Chapter 7. Scales](http://chimera.labs.oreilly.com/books/1230000000345/ch07.html)
    - This chapter helped trmendously with understanding all the little details about how scales work. Input domain –> output range!
* [ ] [D3 and Canvas in 3 steps](https://medium.freecodecamp.com/d3-and-canvas-in-3-steps-8505c8b27444)
* [ ] [The SVG `path` Syntax: An Illustrated Guide](https://css-tricks.com/svg-path-syntax-illustrated-guide/)
* [ ] [Introducing d3-shape](https://medium.com/@mbostock/introducing-d3-shape-73f8367e6d12)
* [ ] [SVGs beyond mere shapes](https://www.visualcinnamon.com/2016/04/svg-beyond-mere-shapes.html)
    - The 30 min video is a good introduction into the examples on the site.
* [ ] [Hacking statistics or: How I Learned to Stop Worrying About Calculus and Love Stats Exercises (Part-2)](http://www.r-exercises.com/2017/07/08/hacking-statistics-exercises-part-2/)
* [x] [Making of: Line drawing on a grid](http://www.redblobgames.com/making-of/line-drawing/)
* [x] [A visual introduction to machine learning](http://www.r2d3.us/visual-intro-to-machine-learning-part-1/)
    - An awesome animated introduction into machine learning concepts implemented with d3.js. Scroll your way through the explanations and see them visualized and animated next to the text while your reading. A great way to publish a presentation-like publication.
* [ ] [📺 (45m) Eyeo 2013 - Bill Atkinson](https://vimeo.com/70630277) — *This is likely not realted to d3 or DataViz at all, but I'll leave it here until I find out.*

Resources
* [Distill](http://distill.pub) — Presents machine learning research in clear, dynamic and vivid ways.
* [Data Sketches](http://www.datasketch.es) — Monthly visualization projects as collaboration between two designers.
* [The Pudding](https://pudding.cool) — Journal of visual essays.
* [Superforecasting](http://goodjudgment.com/superforecasting/index.php/category/superforecasting/)
* [Bl.ock Builder](http://blockbuilder.org) — A web-based development environment for creating d3 visualizations.
    
### Procedural Generation / Generative Art
* [ ] [The Range of Perlin Noise](http://digitalfreepen.com/2017/06/20/range-perlin-noise.html)
* [ ] [Consistent Distance Fields for Ray Marching](http://digitalfreepen.com/2017/06/21/consistent-distance-fields.html)
* [ ] [Restricted Perlin Noise for Better Rendering](http://digitalfreepen.com/2017/06/22/restricted-perlin-noise.html)
* [ ] [Fast and Mostly Consistent Distance Field Ray Marching](http://digitalfreepen.com/2017/06/23/fast-mostly-consistent.html)
* [ ] [Pixel City: Procedurally Generated City in OpenGL](http://www.geeks3d.com/20090615/pixel-city-procedurally-generated-city-in-opengl/)
* [ ] [How to Choose Colours Procedurally (Algorithms)](http://devmag.org.za/2012/07/29/how-to-choose-colours-procedurally-algorithms/)
* [x] [Improved Alpha-Tested Magnification for Vector Textures and Special Effects](http://www.valvesoftware.com/publications/2007/SIGGRAPH2007_AlphaTestedMagnification.pdf)
* [x] [Rendering Text in Metal with Signed-Distance Fields](http://metalbyexample.com/rendering-text-in-metal-with-signed-distance-fields/)
* [ ] [Anti-aliased Euclidean distance transform](http://weber.itn.liu.se/~stegu/aadist/edtaa_preprint.pdf)
* [ ] [A General Algorithm for Computing Distance Transforms in Linear Time](http://fab.cba.mit.edu/classes/S62.12/docs/Meijster_distance.pdf)
* [ ] [So you want to build a generator…](http://galaxykate0.tumblr.com/post/139774965871/so-you-want-to-build-a-generator)
* [ ] [How Unexplored generates great roguelike dungeons](https://www.rockpapershotgun.com/2017/03/10/how-unexplored-generates-great-roguelike-dungeons/)
* [ ] [A Logical Approach to Building Dungeons: Answer Set Programming for Hierarchical Procedural Content Generation in Roguelike Games](http://doc.gold.ac.uk/aisb50/AISB50-S02/AISB50-S2-Smith-paper.pdf)
* [ ] [Representing Game Dialogue as Expressions in First-Order Logic](http://ir.lib.uwo.ca/cgi/viewcontent.cgi?article=2646&context=etd)
* [ ] ? [Data structure for triangle meshes](http://www.redblobgames.com/x/1722-b-rep-triangle-meshes/)
* [ ] ? [Procedural river drainage basins](http://www.redblobgames.com/x/1723-procedural-river-growing/)
* [ ] 📕 Procedural Generation in Games

Resources
* [Awesome Generative Art](https://github.com/kosmos/awesome-generative-art/blob/master/readme.md)
* [Awesome Creative Coding](https://github.com/terkelg/awesome-creative-coding)
* [openframe — a platform for displaying digital art](https://openframe.io)
* [CIS 700 - Special Topics in Procedural Graphics](https://cis700-procedural-graphics.github.io)

### Graphics Programming
* [ ] [📺 (90m) Principles of Lighting and Rendering with John Carmack](https://www.youtube.com/watch?v=IyUgHPs86XM)
* [ ] [The lost art of 3D rendering without shaders](http://machinethink.net/blog/3d-rendering-without-shaders/)
* [ ] [📕 The Book of Shaders](http://thebookofshaders.com)
* [Pixel Spirit Deck](http://pixelspiritdeck.com)
* [Code Tutorials and Experiments: HTML5 Canvas, JavaScript, Processing. • Rectangle World](http://rectangleworld.com/blog/)
* [ ] [A Mind Is Born](https://www.linusakesson.net/scene/a-mind-is-born/index.php)
* [x] [📕 Calculus Learning Guide • Better Explained](https://betterexplained.com/guides/calculus/)
    - *Apart from being an impressive resource in how to present educational material I consider this helpful for implementing an animation system.*
* [ ] [Working with memory in Metal](http://metalkit.org/2017/04/30/working-with-memory-in-metal.html)
* [ ] [Working with memory in Metal part 2](http://metalkit.org/2017/05/26/working-with-memory-in-metal-part-2.html)
* [ ] [GCN Execution Patterns in Full Screen Passes](https://michaldrobot.com/2014/04/01/gcn-execution-patterns-in-full-screen-passes/)
* [ ] [Hylogen — a language embedded in Haskell for live-coding WebGL fragment shaders](https://hylogen.com)
* [ ] [GPU Performance for Game Artists](http://www.fragmentbuffer.com/gpu-performance-for-game-artists/)
* TODO: Add resources from note "DataViz & Generative Art"

----

## Learn more about decentralized, peer-to-peer technologies; I'm interested in blockchain, but not necessarily for financial use cases
* [x] [📺 (15m) Blockchain 101 - A Visual Demo • YouTube](https://youtu.be/Cc3bdKNYlEM)
    - Quick and simple introduction to what a blockchain is and how it works. No previous knowledge required.
* [x] [(15m) The DCS Triangle](https://blog.bigchaindb.com/the-dcs-triangle-5ce0e9e0f1dc)
    - Analyzes several decentralized systems and puts them in categories based on their properties: level of **D**ecentralization, **C**onsistency, and **S**cale.
* [x] [Deciphering “Silicon Valley”: Should we Build a New Internet?](https://medium.com/@rowantrollope/deciphering-silicon-valley-should-we-build-a-new-internet-678990919139)

Resources
* [OpenGarden MeshKit](https://www.opengarden.com/meshkit.html)

----

## Pair with people who can help me become more productive as a programmer and get better at test-driven development
* [ ] [Why and how you should test your software](https://codewithoutrules.com/2017/03/26/why-how-test-software/)
* [x] [The Two Sides of Writing Testable Code](http://news.realm.io/news/try-swift-brandon-williams-writing-testable-code/)
    <br>Brandon describes a way to turn impure functions with both side effects and co-effects into easily testable pure functions in Swift.

## Experiment with sharing my work in progress — maybe finally blog on a regular basis
* [ ] [📕 The Beginner's Guide to Social Media](https://moz.com/beginners-guide-to-social-media)

Resources
* [Staticman: Static sites with superpowers](https://staticman.net)
* [LICEcap](http://www.cockos.com/licecap/) — Tool to create animated GIFs from screen recordings

## Get an introduction into basic devops and set up CI and some more complex toolchains and production environments with Docker, AWS, and whatever else is recommended
* [ ] [iOS Continous integration: Xcode Server, Jenkins, Travis and fastlane](http://thebugcode.github.io/ios-continous-integration-choosing-a-build-server-and-tooling/)
* [ ] [Cheap Bots, Done Quick!](http://cheapbotsdonequick.com)
* [ ] [AWS Adventures: Part 2 – Infrastructure As Code, Deploying a Microservice](http://jessewarden.com/2017/01/aws-adventures-part-2-infrastructure-as-code-deploying-a-microservice.html)

## Other interesting stuff
* [x] [The Dark Secret at the Heart of AI](https://www.technologyreview.com/s/604087/the-dark-secret-at-the-heart-of-ai/)

Reference
* [programmingtalks.org](https://www.programmingtalks.org)
* [Programming Talks • hellerve on GitHub](https://github.com/hellerve/programming-talks)
* [Mega Project List on GitHub](https://github.com/karan/Projects)
* [An extensive list of interesting open source projects](https://github.com/lk-geimfari/awesomo)

----

## Meta

### Complexity in software development
* [x] [(10m) SICP / What is "Computer Science"?](https://m.youtube.com/watch?v=zQLUPjefuWA)
* [x] [📺 (1h) Greg Wilson - What We Actually Know About Software Development, and Why We Believe It’s True](https://vimeo.com/9270320)
    - In software engineering we claim to have figured out many things, but don't back them up with data and research. In many cases we still don't know what's objectively better, and fall victim to statements that sound clever to us, and confirm our own biases. For real progress in our field we need higher standards for proof.
* [x] [Complexity and Strategy](https://hackernoon.com/complexity-and-strategy-325cd7f59a92)
* [x] [Can Programming Be Liberated from the von Neumann Style? A Functional Style and Its Algebra of Programs](http://worrydream.com/refs/Backus-CanProgrammingBeLiberated.pdf)
    <br>Influential article written in 1978 describing a functional system for computation which sounds a lot like what functional programming languages these days are built on.
* [x] [Systems Past: the only 8 software innovations we actually use](https://davidad.github.io/blog/2014/03/12/the-operating-system-is-out-of-date/)
    <br>Criticizes the lack of innovation in programming and explains that the biggest innovations in the field, like programming languages, operating systems, interactivity, and the Internet have been invented between 1955 and 1970.
* [x] [📺 Hearts and Minds • GDC Vault](http://www.gdcvault.com/play/1020788/Hearts-and)
* [ ] [Toward a Galvanizing Definition of Technical Debt](https://michaelfeathers.silvrback.com/toward-a-galvanizing-definition-of-technical-debt)
* [ ] 📕 Mindstorms - Children, Computers, and Powerful Ideas
* TODO: Add resources from note "Reducing Complexity"

Bret Victor material I want to re-watch/read
* [ ] [Mar 2006 • Magic Ink](http://worrydream.com/#!/MagicInk)
* [ ] [Apr 2007 • Substroke](http://worrydream.com/#!/substroke)
* [ ] [Oct 2009 • Simulation as a Practical Tool](http://worrydream.com/#!/SimulationAsAPracticalTool)
* [ ] [Mar 2010 • Ten Brighter Ideas](http://worrydream.com/#!/TenBrighterIdeas)
* [ ] [Mar 2011 • Explorable Explanations](http://worrydream.com/#!/ExplorableExplanations)
* [ ] [Mar 2011 • Dynamic Pictures](http://worrydream.com/#!/DynamicPicturesMotivation)
* [ ] [Apr 2011 • Kill Math](http://worrydream.com/#!/KillMath)
* [ ] [📺 Interactive Exploration of a Dynamical System](http://worrydream.com/#!/InteractiveExplorationOfADynamicalSystem)
* [ ] [May 2011 • Scientific Communication as Sequential Art](http://worrydream.com/#!/ScientificCommunicationAsSequentialArt)
* [ ] [May 2011 • Scrubbing Calculator](http://worrydream.com/#!/ScrubbingCalculator)
* [ ] [Oct 2011 • Up and Down the Ladder of Abstraction](http://worrydream.com/#!2/LadderOfAbstraction)
* [ ] [Nov 2011 • A Brief Rand on the Future of Interaction Design](http://worrydream.com/#!/ABriefRantOnTheFutureOfInteractionDesign)
* [x] [📺 Jan 2012 • Inventing on Principle](http://worrydream.com/#!/InventingOnPrinciple)
    <br>Software Engineers can right wrongs by inventing. Bret's principle is: tools for visual art need immediate feedback. Find yours and change the world.
* [ ] [Sep 2012 • Learnable Programming](http://worrydream.com/#!/LearnableProgramming)
    <br>
* [x] [📺 Nov 2012 • Stop Drawing Dead Fish](http://worrydream.com/#!/StopDrawingDeadFish)
    <br>Impressive demo of how geographical representation can replace symbolic representation for creating graphics, animations, and behavior in a simulation. We're stuck with simulating old media with our new media and don't take advantage of all the capabilities new media offers. Computers should be used for simulations, not just static images, or animations.
* [ ] [📺 Feb 2013 • Drawing Dynamic Visualizations](http://worrydream.com/#!/DrawingDynamicVisualizationsTalk)
* [ ] [📺 Apr 2013 • Media for Thinking the Unthinkable](http://worrydream.com/#!/MediaForThinkingTheUnthinkable)
* [ ] [📺 Jul 2013 • The Future of Programming](http://worrydream.com/#!/TheFutureOfProgramming)
* [ ] [📺 May 2014 • Seeing Spaces](http://worrydream.com/#!/SeeingSpaces)
* [ ] [📺 Oct 2014 • The Humane Representation of Thought](http://worrydream.com/#!/TheHumaneRepresentationOfThoughtTalk)
* [ ] [Nov 2015 • What Can a Technologist Do about Climate Change?](http://worrydream.com/#!/ClimateChange)

### Future of Programming
* [x] [The Hundred-Year Language](http://www.paulgraham.com/hundred.html)
    <br>Abstract thoughts about what programming languages look like in 100 years from now.
* [x] [Toward a frozen operating system](https://urbit.org/blog/2017.5-frozen/)
    <br>Is it possible to build system software or OS level software than never has to be updated?
* [x] [Expressive Programming in VR](http://elevr.com/expressive-programming-in-vr/)
    <br>A very playful demo of how programming in VR could look like.
* [x] [Ask HN: Why does visual programming suck?](https://news.ycombinator.com/item?id=14482988)
    <br>Huge thread about the pros and cons of visual programming interfaces.
* [x] [Resources for creating front-end programming languages and frameworks in 2017](https://medium.com/@stevekrouse/resources-for-creating-front-end-programming-languages-and-frameworks-in-2017-a0c097625f9d)
* [x] [Prune: A Code Editor that is Not a Text Editor](https://www.facebook.com/notes/kent-beck/prune-a-code-editor-that-is-not-a-text-editor/1012061842160013/)
    <br>Post-mortem (unfortunately without any code or even screenshots) of a tree-based code editor prototype that only allows syntactically correct programs through tree transformations.
* [x] [Types are shapes — a graphical programming exploration](https://stevekrouse.com/types-are-shapes-d6af1e83192f)
    <br>Representing different types visually as different shapes helps intuitively understand how types interact with each other. Types are a help for beginners, not an obstacle for experts.
* [x] [WoofJS — making JavaScript learnable](https://stevekrouse.com/woof-d9adf2110fc6)
    <br>A visual programming framework inspired by Sketch, but taking it much further into the web development world. Based on JavaScript.
* [x] [The Rose Project (March 2017) - Making programming better](https://stevekrouse.com/rose-983dc5e0908f)
* [ ] [Flowsheets and Other Observations On Programming Computers](http://tinyletter.com/Flowsheets/archive)
* [ ] [Future Programming Workshop 2014 final videos](http://www.future-programming.org/2014/program.html)
* [ ] [Future Programming Workshop Strange Loop Sep 24, 2015](http://www.future-programming.org/2015/programSL.html)
* [ ] [Future Programming Workshop SPLASH Oct 26-27, 2015](http://www.future-programming.org/2015/programSPLASH.html)
* [ ] [The Gamma: Tools for open data-driven storytelling](https://thegamma.net)
* [ ] [Imp = Spreadsheets + Relations + Time](https://github.com/jamii/imp)
* [ ] [Sourcegraph: Code search + intelligence](https://about.sourcegraph.com)
* [ ] [Human-Centered Programming Tools: Spring 2017 Class Readings](http://pgbovine.net/human-centered-programming-tools.htm)
* [x] [Toby Schachman](http://tobyschachman.com)
* [x] [The Three Projections of Doctor Futamura](http://blog.sigfpe.com/2009/05/three-projections-of-doctor-futamura.html)
    <br>Explains the concept of abstracting over interpreters and compilers and generate specializers that emit interpreters and compilers.
* [x] [Graal & Truffle](https://blog.plan99.net/graal-truffle-134d8f28fb69>)
    <br>Research project to use Futamura projections to create new programming languages quicker which integrate into existing languages and platforms and still perform well.

Resources
* [Human Advancement Research Community](http://harc.ycr.org)
* [📺 Strange Loop Conference Videos](https://www.youtube.com/channel/UC_QIfHvN9auy2CoOdSfMWDw?app=desktop)
* [Visual Programming Languages - Snapshots](http://blog.interfacevision.com/design/design-visual-progarmming-languages-snapshots/)

List of related projects
* [A cross-platform source explorer for C/C++ and Java](https://www.sourcetrail.com/)
* [Luna — Visual and textual functional programming language with a focus on productivity, collaboration and development ergonomics](http://www.luna-lang.org)
* [Bubble — powerful general-purpose visual framework for creating web applications](https://bubble.is)
* [Cirru – An editor for AST](http://cirru.org/)
* [Eve — modern relational language for writing data-driven programs](http://witheve.com) [(Dev Diary)](http://incidentalcomplexity.com)
* [Lamdu - towards a new programming experience](http://www.lamdu.org/)
* [Prune: A Code Editor that is Not a Text Editor](https://www.facebook.com/notes/kent-beck/prune-a-code-editor-that-is-not-a-text-editor/1012061842160013/)
* [MPS Meta Progamming System](http://jetbrains.com/mps)
* https://github.com/cxxtree/cxxtree
* [Frame-based Editing](http://www.greenfoot.org/frames/)
* [Unison — next-generation programming platform](http://unisonweb.org/)
* [Structured editing minor mode for Haskell in Emacs](https://github.com/chrisdone/structured-haskell-mode)
* [ParEdit — minor mode for performing structured editing of S-expression data](https://www.emacswiki.org/emacs/ParEdit)
* [ProjecturEd — generic purpose projectional editor](http://projectured.org)
* more links in [this Hacker News thread](https://news.ycombinator.com/item?id=13773813)

### Stay Focused and Organized

#### A recipe for learning better
1. Get to the point. What do I get from learning the material? Compact lessons, broken up in bite-sized pieces.
2. Have a natural order. Material is taught in an order that supports learning. Can be chronological, is usually gradually increasing complexity and difficulty.
3. Use analogies and visualizations. Avoid abstract concepts and turn them into concrete examples.
4. Make it fun. Avoid top-down lecturing, have a relaxed conversation between peers.

from [Learn Difficult Concepts with the ADEPT Method • betterexplained.com](https://betterexplained.com/articles/adept-method/)

* [x] [📺 (10m) How I plan my week (KanbanFlow)](https://m.youtube.com/watch?v=W9k0OhJkjQ0)
    - Simple personal management technique based in Kanban and Pomodoro to plan your day and week.

Resources
* [SuperBetter - Live Gamefully](https://www.superbetter.com)
