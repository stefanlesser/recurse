# How to Learn Functional Programming
One of my main goals at the [Recurse Center](https://www.recurse.com) was to learn functional programming with Haskell. During the 3-month retreat, I spent plenty of time on reading tutorials, papers, and books about Haskell, functional programming in general, and category theory. Of course, there are always more articles to read and more videos to watch. I went through [a lot of material](https://github.com/stefanlesser/recurse/blob/master/resources/functional-programming.md "My resource collection on functional programming"), and — naturally — some resources are better than others. To make it easier for those who also want to explore the world of functional programming, I present my *ultimate guide to learn functional programming with Haskell*.

---- 

## Getting Started

### [Functional Programming Basics — What’s It All About?](https://pragprog.com/magazines/2013-01/functional-programming-basics)
Robert C. Martin (aka Uncle Bob) • January 2010 • 1883 words

The world of functional programming is huge and complex and full of academic jargon. It is hard to find approachable, practical texts that break down the most important ideas and (over)simplify to help you ease into the subject. Robert breaks the most important concepts down for you in a quick read and sets the stage for a new way to think about writing programs — without assignment statements. There is much more to functional programming than just that, but it’s a great starting point.

### [Functional programming patterns for the non-mathematician (cut)](https://www.youtube.com/watch?v=AvgwKjTPMmM)
Brian Lonsdorf (aka DrBoolean) • April 2014 • 30 mins

Before you try to understand abstract concepts like functors and monads, it’s often good to see the benefits of using these concepts in practice. Brian takes you on a whirlwind tour of how composition, lenses, monoids, functors, applicatives, and monads help you with nesting (a way to compose), null checking (with Maybe), error handling (with Either), and accumulation (reduce) in JavaScript. Even if you don’t understand the words and concepts (yet), you get a glimpse into the power these concepts provide.

### [Professor Frisby's Mostly Adequate Guide to Functional Programming](https://drboolean.gitbooks.io/mostly-adequate-guide/content/)
Brian Lonsdorf (aka DrBoolean) • work in progress • 10+ chapters

Even if you ultimately want to get into a pure functional programming language, I suggest starting with this guide for JavaScript. It explains all the important concepts in a very approachable and practical way, and is relatively short to work through. And because you likely already know JavaScript, you don’t have to deal with foreign syntax or set up a new toolchain to get started.

## Learning Haskell

### [PureScript by Example](https://leanpub.com/purescript/read)
Phil Freeman • December 2016 • 14 chapters

Wait, wasn’t this about learning Haskell?! What is PureScript? — Right, this might seem a little weird, but trust me on this. There’s many books on Haskell, and I will recommend one below, but you might be better off learning PureScript first. PureScript’s syntax is almost identical to Haskell, and the differences between the two languages are not important, if you just start learning them. In a way PureScript even feels like a more cleaned-up version of Haskell, because it’s relatively new and doesn’t have to carry the history and baggage of a language like Haskell. Also, this book is very practical and avoids the academic mannerisms you’ll have to get comfortable with in Haskell-land.

### [Getting started with Haskell • Stack Overflow](https://stackoverflow.com/questions/1012573/getting-started-with-haskell/1016986#1016986)
Answer by David Miani • updated June 2017 • 1871 words

Ok, getting ready for the real thing, David’s answer on Stack Overflow shows you the path to learning Haskell. He outlines the progression from beginner to expert, links to several excellent resources, and sets expectations. If you worked through all the resources above, you’re more than ready to go on this journey, and this is the final reality check to gauge if this trip will really take you where you want to go.

### [Haskell Programming from First Principles](http://haskellbook.com)
Christopher Allen, Julie Moronuki • 31 chapters

Of all the Haskell books I tried, this is the one I recommend. It is more academic than every other resource above, but still approachable. It starts off with a very abstract introduction to lambda calculus, which is an important basis to know about before diving into Haskell. It does make the first chapter a little strange — keep reading and don't judge the book until after chapter 2. This is a massive book with lots of depth. It is useful to work through it cover to cover and spend some time with the exercises to truly understand all concepts. With the knowledge from the resources above you should be prepared for everything this book throws at you. Good luck!

## Applying Functional Concepts

### [Monoids, Functors, Applicatives, and Monads: 10 Main Ideas](https://monadmadness.wordpress.com/2015/01/02/monoids-functors-applicatives-and-monads-10-main-ideas/)
Siddharth Trehan • January 2015 • 3445 words

I found this article one of the best resources on the four big structures in functional programming. If you’re struggling with grasping these concepts, this article might provide a different perspective to get you to your aha-moment. It is also a great resource to go back to when you need a refresher.

### [Haskell Typeclassopedia](https://wiki.haskell.org/Typeclassopedia)
Brent Yorgey • March 2009 • 23466 words

Haskell’s main trick is to pull out fairly abstract patterns and implement them as concrete type classes. Here you’ll find detailed descriptions of all these type classes and this will likely become your ultimate resource to understand them in full detail.

### [What I Wish I Knew When Learning Haskell](http://dev.stephendiehl.com/hask/)
Stephen Diehl • 85857 words

If you start using Haskell to actually write real programs, this huge collection of useful tips will make your day-to-day development with Haskell much easier. Here you can find anything from how to set up your editor for Haskell to implementation details about Haskell’s compiler.

## Category Theory

### [Haskell/Category theory](https://en.wikibooks.org/wiki/Haskell/Category_theory)
May 2017 • 4047 words

If your cravings for abstraction are still not satisfied at this point, you can use this chapter as an introduction to category theory. Personally, I doubt that you really need this for becoming a productive functional programmer, but if you seek enlightenment this can put you on your next path.

---- 

This is my list of recommended resources for learning functional programming and Haskell (+ PureScript). I’ve compiled this list from [a much bigger list of material I worked through](https://github.com/stefanlesser/recurse/blob/master/resources/functional-programming.md), but of course it is likely that you might find something even better. If you think this list needs an update because you found a book, an article, or a video that is so much better than anything on this list, please let me know and [get in touch](https://twitter.com/stefanlesser)!
