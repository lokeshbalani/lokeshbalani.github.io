# Garbage Collection and Memory Management in JavaScript

## Introduction

JavaScript automatically allocates memory when objects are created and frees it when they are not used anymore (garbage collection). This seemingly “automatical” nature of freeing up resources is a source of confusion and gives JavaScript (and other high-level-language) developers the false impression they can choose not to care about memory management. This is a big mistake.

## Memory Life Cycle

Regardless of the programming language, memory life cycle is pretty much always the same:

1. Allocate the memory you need
2. Use the allocated memory (read, write)
3. Release the allocated memory when it is not needed anymore

The second part is explicit in all languages. The first and last parts are explicit in low-level languages but are mostly implicit in high-level languages like JavaScript.

**Allocate Memory**  
Memory is allocated by the operating system which allows the program to use it. In low-level languages (e.g. C) this is an explicit operation that a developer should handle. In high-level languages, however, this is taken care of automamtically.

**Use Memory**  
This is the time when the program actually makes use of the previously allocated memory. Read and write operations are taking place as program uses allocated variables in code.

**Release Memory**  
Release the entire memory that is not needed so that it can become free and available again.

Poor coding may lead to memory leaks, which is a condition where memory is not released even though it is no longer used by the application. So it is very important to learn more about memory management

## Memory Leaks

Memory leaks are a problem every developer has to face. Leaks are the cause of whole class of problems: slowdowns, crashes, high latency, and even problems with other applications.

**What are Memory Leaks?**  
Memory leaks can be defined as memory that is not required by an application anymore that for some reason is not returned to the operating system or the pool of free memory.