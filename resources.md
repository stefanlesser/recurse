# Study Resources
_My big dumping ground for links to articles, (e)books, videos and similar material that caught my attention, but I haven't had the time to look at yet. I'm still figuring out how to work with this list…_

----

## Dive into advanced functional programming concepts with Haskell and Swift
See [here](resources/functional-programming.md)

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
* [ ] [📺 (40m) How to write a Turing-Complete Programming Language in 40 minutes](https://www.youtube.com/watch?v=_Uoyufkb5lk)
* [x] [📺 (40m) Andy Keep - Writing a Nanopass Compiler](https://www.youtube.com/watch?v=Os7FE3J-U5Q&t=2s)
    <br>Introduction to the technique of contructing compilers as a sequence of tiny translation passes.
* [ ] [An Incremental Approach to Compiler Construction](http://scheme2006.cs.uchicago.edu/11-ghuloum.pdf)
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
* [ ] 📕 Concepts, Techniques, and Models of Computer Programming
* [ ] [The memory models that underlie programming languages • canonical.org](http://canonical.org/~kragen/memory-models/)
* [ ] [📺 (45m) Modelica: Component Oriented Modeling of Physical Systems" by Michael Tiller](https://www.youtube.com/watch?v=-mvEUuc-sWE)
* [ ] [📺 (45m) Ceptre: A Language for Modeling Generative Interactive Systems" by Chris Martens](https://www.youtube.com/watch?v=bFeJZRdhKcI)

### Parsing
* [ ] [Monadic Parsers: Implementing a micro Parsec](http://olenhad.me/articles/monadic-parsers/)
* [ ] [Swift Talk #13 Parsing Techniques](https://talk.objc.io/episodes/S01E13-parsing-techniques)
* [ ] [Parsing context-sensitive languages with Applicative](https://byorgey.wordpress.com/2012/01/05/parsing-context-sensitive-languages-with-applicative/)
* [x] [A Tutorial Explaining LALR(1) Parsing](https://web.cs.dal.ca/~sjackson/lalr1.html)
    <br>Detailed walk-through of how to implement a parser based on a bottom-up approach.
* [x] [Earley Parsing Explained](http://loup-vaillant.fr/tutorials/earley-parsing/)
    - In-depth walk-through of how Early parsing works. Code samples in Lua.
* [ ] [Bounded Seas — Island Parsing Without Shipwrecks](http://scg.unibe.ch/archive/papers/Kurs14b-BoundedSeas.pdf)

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
* [x] [How to follow the JavaScript roadmap](https://benmccormick.org/2017/07/10/how-to-follow-the-javascript-roadmap/)
* [x] [Overview of ECMAScript 6 features](https://github.com/lukehoban/es6features)
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
* [Awesome Dataviz](https://github.com/fasouto/awesome-dataviz)
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
* [x] [📺 (30m) Big picture software testing unit testing, Lean Startup, and everything in between](https://www.youtube.com/watch?v=Vaq_e7qUA-4&feature=youtu.be&t=63s)
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
* [Programming books you might want to consider reading](https://danluu.com/programming-books/)
* [Mega Project List on GitHub](https://github.com/karan/Projects)
* [An extensive list of interesting open source projects](https://github.com/lk-geimfari/awesomo)

----

## Meta

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
