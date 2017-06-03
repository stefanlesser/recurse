# Study Resources
_My big dumping ground for links to articles, (e)books, videos and similar material that caught my attention, but I haven't had the time to look at yet. I'm still figuring out how to work with this list…_

Resources marked with ★ are recommended starting points or must read|watch material for the given category.

----

## Project Ideas

### Dive into advanced functional programming concepts with Haskell and Swift
* [x] [★ Functional Programming Basics - What’s It All About?](https://pragprog.com/magazines/2013-01/functional-programming-basics)
    <br>"Functional Programming is progamming without assignment statements." This means data in memory is (mostly) immutable and that makes parallelism for multiple CPU cores much easier to reason about. This article is a very high-level introduction into one of the core concepts of FP and ties it to one of the main benefits. I do think there's more to it than that, but this should get you excited about it.
* [x] [📺 (60m) "I See What You Mean" by Peter Alvaro](https://www.youtube.com/watch?v=R2Aa4PivG0g)
    <br>Entertaining presentation about modeling state with declarative languages. Many applicable concepts although it is understandably a little heavy on the relational language this talk is about.
* [x] [📺 (60m) Category Theory for the Working Hacker by Philip Wadler](https://www.youtube.com/watch?v=V10hzjgoklA)
    <br>If you want to take it an abstraction level higher, this surprisingly entertaining talk explains the math behind lambda calculus called category theory.
* [x] [From Higher-Order Functions to Libraries And Frameworks](http://raganwald.com/2016/12/15/what-higher-order-functions-can-teach-us-about-libraries-and-frameworks.html)
    <br>How higher-order functions influence the expressiveness and complexity of programs. This is part 1 of a series of 3 articles.
* [x] [Functional Programming is taking over UIs with Pure Views](https://medium.freecodecamp.com/the-revolution-of-pure-views-aed339db7da4)
    <br>Why functional programing helps keeping the user interface layer simple and enables hot module replacement, time-travel debugging and similar features.
* [x] [A Beginner-Friendly Tour through Functional Programming in Scala](http://degoes.net/articles/easy-monads)
    <br>Introduces benefits of functional programming by transforming a simple console program from imperative to declarative step by step. Even though it's using Scala, it helps understanding the basic building blocks of FP and their benefits.
* [x] [Destroy All Ifs — A Perspective from Functional Programming](http://degoes.net/articles/destroy-all-ifs)
    <br>By replacing conditionals with lambdas, we can invert control and make our code both easier to reason about and more generic. Moving conditionals from places hidden in the deepest nested function up to the caller makes intent clear and prevents mistakes.
* [ ] [A Modern Architecture for FP](http://degoes.net/articles/modern-fp)
* [ ] [Modern Functional Programming: Part 2](http://degoes.net/articles/modern-fp-part-2)
* [ ] [Queer Types - Applicatives and Alternatives](https://queertypes.com/posts/59-applicatives-alternatives.html)
* [ ] [Writing Video Games in a Functional Style](http://prog21.dadgum.com/228.html)
* [ ] 📕 Modeling Data with Functional Programming in R

#### Haskell
* [ ] (45% done) [★ 📕 Haskell Programming from First Principles](http://haskellbook.com)
    <br>So far I like this book much better than the free "Learn you a Haskell". It starts off with a very abstract introduction to lambda calculus, which I believe is an important basis to know about before diving into Haskell. It does make the first chapter a little strange — keep reading and don't judge the book until after chapter 2.
* [x] [📺 (60m) Gabriel Gonzales: Applied category theory and abstract algebra - λC Winter Retreat 2017](https://www.youtube.com/watch?v=WsA7GtUQeB8)
    <br>"[We can] tackle software complexity by reusing standard interfaces that originate in the fields of category theory and abstract algebra." Builds understanding for composition going from composable functions to composable values (monoids) to composable types (applicatives) and shows how powerful these concepts are to decompose programs into simple building blocks.
* [x] [The category design pattern](http://www.haskellforall.com/2012/08/the-category-design-pattern.html)
* [ ] [The functor design pattern](http://www.haskellforall.com/2012/09/the-functor-design-pattern.html)
* [ ] [Data is Code](http://www.haskellforall.com/2016/04/data-is-code.html?m=1)
* [ ] [📺 (2h:15m) Phil Freeman - Fun with Profunctors](https://www.youtube.com/watch?v=OJtGECfksds)
* [ ] [The Y Combinator (Slight Return) or How to Succeed at Recursion Without Really Recursing](http://mvanier.livejournal.com/2897.html)
* [ ] [7 lines of code, 3 minutes: Implement a programming language from scratch](http://matt.might.net/articles/implementing-a-programming-language/)
* [ ] [Closure conversion: How to compile lambda](http://matt.might.net/articles/closure-conversion/)
* [ ] [Compiling to lambda-calculus: Turtles all the way down](http://matt.might.net/articles/compiling-up-to-lambda-calculus/)
* [ ] [Equational derivations of the Y combinator and Church encodings in Python](http://matt.might.net/articles/python-church-y-combinator/)
* [ ] [Fixed-point combinators in JavaScript: Memoizing recursive functions](http://matt.might.net/articles/implementation-of-recursive-fixed-point-y-combinator-in-javascript-for-memoization/)
* [ ] [Haskell Communities and Activities Report • 32nd Ed. May 2017](https://www.haskell.org/communities/05-2017/html/report.html)
* TODO: select RC Wiki Haskell resources

#### Swift
* [x] [📺 (45m) Brandon Williams - Finding Happiness in Functional Programming](https://www.youtube.com/watch?v=A0VaIKK2ijM)
    <br>Exploring the benefits and downsides of functional conepts in practical use, from isolation of side (and co-)effects to coding for an interface we wish we had instead of the one we're given. Great points about how to encapsulate state management with lenses using UIKit as an example.
* [ ] (20% done) [📺 (10 Talks) Functional Swift Conference 2017](http://2017.funswiftconf.com)
* [x] [📺 (40m) Brandon Kase: Beyond Types in Swift](https://m.youtube.com/watch?v=6z9QjDUKkCs)
    <br>Adding functionality without adding complexity through abstract algebra:
    - Magma: closed binary operators = composable operation
    - Semi-group: + associativity = parallelization
    - Monoid: + identity = dropping the optional
    - Commutative Monoid: + commutativity = reorder
    - Bounded Semilattice: + idempotence = no need for memory
* [x] [📺 (40m) Monoids, Predicates and Sorting Functions](https://www.youtube.com/watch?v=VFPhPOnPiTY)
    <br>This demonstrates the practical application of the other Brandon's talk above with live coding in Swift Playgrgounds. Impressive composability of the simplest components by building them up following the rules and laws.
* [x] [Swift Enums Are "sum" Types. That Makes Them Very Interesting](https://mislavjavor.github.io/2017-04-19/Swift-enums-are-sum-types.-That-makes-them-very-interesting/)
    <br>Explains product and sum types and shows how they can be used to minimize possible use cases and define away potential error states. With examples for use cases for sum types (enums) like router and theme patterns and tree data structures.
* [x] [Algebraic Structure and Protocols](http://www.fewbutripe.com/swift/math/algebra/2015/02/17/algebraic-structure-and-protocols.html)
    <br>This article takes a mathmatical approach to introduce monads through semigroups.
* [x] [The Algebra of Predicates and Sorting Functions](http://www.fewbutripe.com/swift/math/algebra/monoid/2017/04/18/algbera-of-predicates-and-sorting-functions.html)
    <br>Extends the knowledge about semigroups and monoids to introduce predicate and sorting functions.
* [x] [📺 (30m) Brandon Williams - Lenses in Swift](https://www.youtube.com/watch?v=ofjehH9f-CU)
    <br>Using lenses and prisms to create getters and setters for immutable values.

----

### Build a interpreter/compiler and create a simple programming language from scratch
* [x] [Rich Programmer Food](http://steve-yegge.blogspot.com/2007/06/rich-programmer-food.html?m=1)
* [x] [So You Want To Write Your Own Language?](http://www.drdobbs.com/architecture-and-design/so-you-want-to-write-your-own-language/240165488)
    - Focus on: context-free grammar, good diagostics (redundancy helps), tried and true grammatical forms for familiar constructs. Ignore: minimizing keystrokes, easy parsing, minimizing keywords, lexer or parser generators.
    - Use a poisoning approach for marking errors in the AST, like in D.
    - Use a profiler to find performance issues.
    - Take advantage of lowering (rewriting more complex semantic constructs in terms of simpler ones, e.g. while and for-each loops can both be rewritten as for loops).
    - Don't forget that a good runtime library is important. Don't have too much trivia in it.
* [ ] [📕 Crafting Interpreters - A handbook for making programming languages • Bob Nystrom](http://www.craftinginterpreters.com)
* [ ] [Building a Primitive State Machine in Haskell](https://daniel-levin.github.io/2015/01/19/primitive-state-machine-in-haskell.html)
* [ ] [Turing Machines and Tooling, Part I](http://raganwald.com/2017/04/06/turing-machines.html)
* [ ] [Turing Machines and Tooling, Part II](http://raganwald.com/2017/04/16/turing-machines-part-ii.html)
* [ ] [Implementing a JIT Compiled Language with Haskell and LLVM](http://www.stephendiehl.com/llvm/)
* [ ] [Building a LISP from scratch with Swift](https://www.uraimo.com/2017/02/05/building-a-lisp-from-scratch-with-swift/)
* [ ] [The Lambda Calculus for Absolute Dummies (like myself) • palmström](http://palmstroem.blogspot.jp/2012/05/lambda-calculus-for-absolute-dummies.html?m=1)
* [ ] [COMPUTATION STARTING FROM FIRST PRINCIPLES (DRAFT) • Jan Wedekind](http://www.wedesoft.de/binary-lambda-calculus.html)
* [ ] [Implementing a JIT Compiled Language with Haskell and LLVM](http://www.stephendiehl.com/llvm/)
* [x] [Software structure for programmers who know at least one programming language](https://www.destroyallsoftware.com/compendium/software-structure/6fb5f711cae5a4e6)
* [x] [Types for anyone who knows a programming language](https://www.destroyallsoftware.com/compendium/types/baf6b67369843fa2)
    - Introduction to and overview of several different type systems in popular programming languages.
* [ ] [The memory models that underlie programming languages • canonical.org](http://canonical.org/~kragen/memory-models/)
* [ ] [Dragon taming with Tailbiter, a bytecode compiler for Python • codewords.recurse.com](https://codewords.recurse.com/issues/seven/dragon-taming-with-tailbiter-a-bytecode-compiler)
* [ ] [Swift Talk #13 Parsing Techniques](https://talk.objc.io/episodes/S01E13-parsing-techniques)
* [ ] [📺 (45m) Modelica: Component Oriented Modeling of Physical Systems" by Michael Tiller](https://www.youtube.com/watch?v=-mvEUuc-sWE)
* [ ] [📺 (45m) Ceptre: A Language for Modeling Generative Interactive Systems" by Chris Martens](https://www.youtube.com/watch?v=bFeJZRdhKcI)
* [x] [Earley Parsing Explained](http://loup-vaillant.fr/tutorials/earley-parsing/)
    - In-depth walk-through of how Early parsing works. Code samples in Lua.
* [ ] 📕 Concepts, Techniques, and Models of Computer Programming

Resources
* [Earley parser implementation • GitHub](https://github.com/lagodiuk/earley-parser-js)
* [FParsec Documentation](http://www.quanttec.com/fparsec/)

### Brush up my knowledge about (graph) data structures and algorithms
* TODO: add resources from reading list and iBooks

#### Conflict-Free Replicated Data Types (CRDT)
* [ ] [Conflict-free replicated data type](https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type)
* [ ] [A Look at Conflict-Free Replicated Data Types (CRDT)](https://medium.com/@istanbul_techie/a-look-at-conflict-free-replicated-data-types-crdt-221a5f629e7e)
* [ ] [Conflict-free replicated data types](https://medium.com/@qt/a-brief-history-of-replicated-data-ab9dcf1671a0)
* [ ] [Conflict-free Replicated Data Types](http://muratbuffalo.blogspot.com/2013/04/conflict-free-replicated-data-types.html)
* [ ] [A comprehensive study of Convergent and Commutative Replicated Data Types](http://hal.upmc.fr/file/index/docid/555588/filename/techreport.pdf)
* [Readings in conflict-free replicated data types](http://christophermeiklejohn.com/crdt/2014/07/22/readings-in-crdts.html)

### Try (functional) reactive programming with RxSwift and/or React.js
* [ ] [📺 Everyday Reactive](https://news.realm.io/news/everyday-reactive/)
* [ ] [What is reactive programming and why should I use it?](https://www.cocoawithlove.com/blog/reactive-programming-what-and-why.html)
* [ ] [The introduction to Reactive Programming you've been missing](https://gist.github.com/staltz/868e7e9bc2a7b8c1f754)
* [ ] [Reactive programming from scratch](http://www.thomasvisser.me/2016/11/28/reactive-from-scratch/)
* [ ] [Do-It-Yourself Functional Reactive Programming](https://speakerdeck.com/mchakravarty/do-it-yourself-functional-reactive-programming)

### Get back into JavaScript (and possibly TypeScript) and see what’s state of the art for web development (looking at React, Relay, GraphQL, Jest, etc.)
* [x] [Overview of ECMAScript 6 features](https://github.com/lukehoban/es6features)
* [x] [A Functional Programmer’s Introduction to JavaScript (Composing Software)](https://medium.com/javascript-scene/a-functional-programmers-introduction-to-javascript-composing-software-d670d14ede30)
* [ ] [http://jrsinclair.com/articles/2017/javascript-without-loops/index.html](http://jrsinclair.com/articles/2017/javascript-without-loops/index.html)
* [ ] [Higher Order Functions (Composing Software)](https://medium.com/javascript-scene/higher-order-functions-composing-software-5365cf2cbe99)
* [ ] 📕 Eloquent JavaScript

Reference
* [📕 Exploring ES6](http://exploringjs.com/es6/index.html)
* [Design Patterns in ES6](http://tcorral.github.io/Design-Patterns-in-Javascript/)
* [📕 Speaking JavaScript (ES5)](http://speakingjs.com/es5/index.html)

### Explore data visualization, procedural generation, and generative art — I want to try d3.[js|express] and graphics programming with Metal or Vulcan

#### Information Visualization
General
* [ ] [Information Visualization • Enrico Bertini](http://enrico.bertini.io/teaching/)
* [ ] [The death of interactive infographics?](https://medium.com/@dominikus/the-end-of-interactive-visualizations-52c585dcafcb)
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
* [x] [Making of: Line drawing on a grid](http://www.redblobgames.com/making-of/line-drawing/)
* [x] [A visual introduction to machine learning](http://www.r2d3.us/visual-intro-to-machine-learning-part-1/)
    - An awesome animated introduction into machine learning concepts implemented with d3.js. Scroll your way through the explanations and see them visualized and animated next to the text while your reading. A great way to publish a presentation-like publication.
* [ ] [Eyeo 2013 - Bill Atkinson](https://vimeo.com/70630277) — *This is likely not realted to d3 or DataViz at all, but I'll leave it here until I find out.*

Resources
* [Distill](http://distill.pub) — Presents machine learning research in clear, dynamic and vivid ways.
* [Data Sketches](http://www.datasketch.es) — Monthly visualization projects as collaboration between two designers.
* [The Pudding](https://pudding.cool) — Journal of visual essays.
* [Superforecasting](http://goodjudgment.com/superforecasting/index.php/category/superforecasting/)
* [Bl.ock Builder](http://blockbuilder.org) — A web-based development environment for creating d3 visualizations.
    
#### Procedural Generation / Generative Art
* [Awesome Generative Art](https://github.com/kosmos/awesome-generative-art/blob/master/readme.md)
* [ ] [So you want to build a generator…](http://galaxykate0.tumblr.com/post/139774965871/so-you-want-to-build-a-generator)
* [ ] [How Unexplored generates great roguelike dungeons](https://www.rockpapershotgun.com/2017/03/10/how-unexplored-generates-great-roguelike-dungeons/)
* [ ] 📕 Procedural Generation in Games
    
#### Graphics Programming
* [ ] [📺 (90m) Principles of Lighting and Rendering with John Carmack](https://www.youtube.com/watch?v=IyUgHPs86XM)
* [ ] [The lost art of 3D rendering without shaders](http://machinethink.net/blog/3d-rendering-without-shaders/)
* [ ] [📕 The Book of Shaders](http://thebookofshaders.com)
* [Pixel Spirit Deck](http://pixelspiritdeck.com)
* [Code Tutorials and Experiments: HTML5 Canvas, JavaScript, Processing. • Rectangle World](http://rectangleworld.com/blog/)
* [ ] [A Mind Is Born](https://www.linusakesson.net/scene/a-mind-is-born/index.php)
* [x] [📕 Calculus Learning Guide • Better Explained](https://betterexplained.com/guides/calculus/)
    - *Apart from being an impressive resource in how to present educational material I consider this helpful for implementing an animation system.*
* TODO: Add resources from note "DataViz & Generative Art"

### Learn more about decentralized, peer-to-peer technologies; I'm interested in blockchain, but not necessarily for financial use cases
* [x] [📺 (15m) Blockchain 101 - A Visual Demo • YouTube](https://youtu.be/Cc3bdKNYlEM)
    - Quick and simple introduction to what a blockchain is and how it works. No previous knowledge required.
* [x] [(15m) The DCS Triangle](https://blog.bigchaindb.com/the-dcs-triangle-5ce0e9e0f1dc)
    - Analyzes several decentralized systems and puts them in categories based on their properties: level of **D**ecentralization, **C**onsistency, and **S**cale.
* [x] [Deciphering “Silicon Valley”: Should we Build a New Internet?](https://medium.com/@rowantrollope/deciphering-silicon-valley-should-we-build-a-new-internet-678990919139)

Resources
* [OpenGarden MeshKit](https://www.opengarden.com/meshkit.html)

### Pair with people who can help me become more productive as a programmer and get better at test-driven development
* [ ] [Why and how you should test your software](https://codewithoutrules.com/2017/03/26/why-how-test-software/)

### Experiment with sharing my work in progress — maybe finally blog on a regular basis
* [ ] [📕 The Beginner's Guide to Social Media](https://moz.com/beginners-guide-to-social-media)

Resources
* [Staticman: Static sites with superpowers](https://staticman.net)

### Get an introduction into basic devops and set up CI and some more complex toolchains and production environments with Docker, AWS, and whatever else is recommended
* [ ] [iOS Continous integration: Xcode Server, Jenkins, Travis and fastlane](http://thebugcode.github.io/ios-continous-integration-choosing-a-build-server-and-tooling/)
* [ ] [Cheap Bots, Done Quick!](http://cheapbotsdonequick.com)
* [ ] [AWS Adventures: Part 2 – Infrastructure As Code, Deploying a Microservice](http://jessewarden.com/2017/01/aws-adventures-part-2-infrastructure-as-code-deploying-a-microservice.html)

### Other interesting stuff
* [x] [The Dark Secret at the Heart of AI](https://www.technologyreview.com/s/604087/the-dark-secret-at-the-heart-of-ai/)
* [ ] [📺 Everything a Swift Dev Ever Wanted to Know About Machine Learning](https://news.realm.io/news/swift-developer-on-machine-learning-try-swift-2017-gallagher/)
* [ ] [📺 Writing Your UI Swiftly](https://news.realm.io/news/sommer-panage-writing-your-ui-swiftly/)
* [ ] [Building a Gas Pump Scanner with OpenCV/Python/iOS](https://hackernoon.com/building-a-gas-pump-scanner-with-opencv-python-ios-116fe6c9ae8b)

Reference
* [📺 Strange Loop Conference Videos](https://www.youtube.com/channel/UC_QIfHvN9auy2CoOdSfMWDw?app=desktop)
* [An extensive list of interesting open source projects](https://github.com/lk-geimfari/awesomo)

----

## Meta

### A recipe for learning better
1. Get to the point. What do I get from learning the material? Compact lessons, broken up in bite-sized pieces.
2. Have a natural order. Material is taught in an order that supports learning. Can be chronological, is usually gradually increasing complexity and difficulty.
3. Use analogies and visualizations. Avoid abstract concepts and turn them into concrete examples.
4. Make it fun. Avoid top-down lecturing, have a relaxed conversation between peers.

from [Learn Difficult Concepts with the ADEPT Method • betterexplained.com](https://betterexplained.com/articles/adept-method/)

### Complexity in software development
* [x] [(10m) SICP / What is "Computer Science"?](https://m.youtube.com/watch?v=zQLUPjefuWA)
* [x] [📺 (1h) Greg Wilson - What We Actually Know About Software Development, and Why We Believe It’s True](https://vimeo.com/9270320)
    - In software engineering we claim to have figured out many things, but don't back them up with data and research. In many cases we still don't know what's objectively better, and fall victim to statements that sound clever to us, and confirm our own biases. For real progress in our field we need higher standards for proof.
* [x] [Complexity and Strategy](https://hackernoon.com/complexity-and-strategy-325cd7f59a92)
* [ ] [Can Programming Be Liberated from the von Neumann Style? A Functional Style and Its Algebra of Programs](http://worrydream.com/refs/Backus-CanProgrammingBeLiberated.pdf)
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
* [ ] [📺 Jan 2012 • Inventing on Principle](http://worrydream.com/#!/InventingOnPrinciple)
* [ ] [Sep 2012 • Learnable Programming](http://worrydream.com/#!/LearnableProgramming)
* [ ] [📺 Nov 2012 • Stop Drawing Dead Fish](http://worrydream.com/#!/StopDrawingDeadFish)
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
* [ ] [Expressive Programming in VR](http://elevr.com/expressive-programming-in-vr/)

### Stay Focused and Organized
* [x] [📺 (10m) How I plan my week (KanbanFlow)](https://m.youtube.com/watch?v=W9k0OhJkjQ0)
    - Simple personal management technique based in Kanban and Pomodoro to plan your day and week.

Resources
* [SuperBetter - Live Gamefully](https://www.superbetter.com)
