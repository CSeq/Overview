


# <img src="logo.png" width="75">: A Family of Sequentialization-Based C Verification Tools

Sequentialization is a technique for the analysis of concurrent programs that exploits verification techniques or tools that were originally designed for sequential programs. Sequentialization can be implemented as a code-to-code translation from the concurrent program into a corresponding non-deterministic sequential program that simulates all executions of the original program. The sequential program contains both the mapping of the threads in the form of functions, and an encoding of the scheduler, where the non-determinism allows to handle different concurrent schedules collectively.
This approach has three main advantages:

    a code-to-code translation is typically much easier to implement than a full-fledged analysis tool;
    it allows designers to focus only on the concurrency aspects of programs, delegating all sequential reasoning to an existing target analysis tool;
    sequentializations can be designed to target multiple backends for sequential program analysis.

CSeq is a framework that facilitates the development of code-to-code translations for concurrent C programs with POSIX threads based on sequentialization. 
