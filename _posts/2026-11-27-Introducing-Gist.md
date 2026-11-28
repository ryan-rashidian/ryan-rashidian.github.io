---
layout: post
title: "Introducing Gist: My Lisp Interpreter"
author: "Ryan Rashidian"
tags: [programming]
---

***

This project is still in early stages of development, but I plan to start a public repository soon (maybe the first day of 2027) where anyone can compile and check it out.

# Introduction

Gist is a small Lisp based on the R5RS specification for Scheme, and the interpreter is written entirely in C (C99). I was inspired to start this project after following a long rabbit hole that ended in reading "Crafting Interpreters" by Robert Nystrom. As a result, the code follows a similar structure to the interpreter in the second part of that book.

Gist has a bytecode compiler paired together with a stack based virtual machine, and borrows the concept of an `upvalue` from Lua. Features such as "tail call optimization" (TCO) and many of the primitives and special forms expected in a proper Lisp have been implemented already, with more planned for the future.

# Goal

The goal for this project is simple: to build a working programming language, and learn some things along the way. There will be absolutely no AI generated code in the interpreter, as that would defeat the purpose. There is no deadline, no shareholders, no use case for a another Lisp in a sea of them already made. Everything will be researched from published, or otherwise credible sources. Though the language will be based on the R5RS standard, I have not decided whether I will strictly adhere to it, or seek to be fully compliant with it.

There are other ideas for the project that may, or may not be added once the foundation is solid. Such as making a C library that compiles the interpreter for embedding purposes. But the initial focus will be on making a fast, light weight interpreter with an easily extendable code-base.

# Research

As mentioned in the introduction, "Crafting Interpreters" by Robert Nystrom is heavily referenced for this project, as well as "Structure and Interpretation of Computer Programs" by Abelson and Sussman (SICP), and the R5RS itself. Anyone familiar with one or more of those materials should be able to follow along with this project's development.

***

