---
layout: post
title: "Estopp that Man!"
date: 2013-04-14 15:51
comments: true
categories: Programming 
---

<p>Ever had your heart broken by promises that were left unfulfilled? In legal
theory there's a concept called "Estoppel" that precludes someone from escaping
from the consequences of their promises, even if the promises are informal and
not technically legally binding. In other words, even if you didn't sign a
contract saying you'd do something, if someone's counting on you to do that
thing, you can't get out of it just because you didn't squiggle your name on a
piece of paper.</p>
<p>I encountered this concept last semester in my jurisprudence class, and I've
got to say, I wish we had a similar concept in computer programming. I think
everyone can agree the most frustrating parts of dynamic languages is their lack
of explicit contracts between functions. In Python, for instance, you have to
explicitly document what you expect each function to take in and output. If you
don't you get bizarre, often silent, errors. In C, however, the prototype of
each function declares a certain type contract you must abide by.</p>
<p>So how does the average Python programmer deal with an implicit type
contract? Usually I see docstrings that beg for proper usage, or for simpler
programs nothing at all in the hopes that anyone smart enough can decipher the
purpose and requirements of their code. I'm not satisfied with this! In legal
terms there's nothing estopping (that's how you say it!) a developer to change
their program's contracts (except perhaps the ever-present-but-low probability that
one of their users is an axe-murderer!).</p>
<p>I propose a solution to the un-estoppe-able tragedy of dynamic languages: algorithmically making
explicit the dependencies of functions and printing these dependencies in the
prototype of functions. In other words, you can have the benefit of dynamic
languages as you're writing your program, but when it's time to publish to
Github, a program either discovers your functions' dependencies or prompts you
to declare them and then makes it easy for other developers to understand your
code.</p>
