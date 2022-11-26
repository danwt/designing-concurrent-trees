# designing-concurrent-trees

**My MSc thesis on designing correct concurrent shared memory balance tree data structures, with the help of model checking and TLA+.**

[![Blog](https://img.shields.io/badge/-.pdf-informational?style=flat-square&logo=adobe-acrobat-reader&logoColor=white)](https://github.com/danwt/designing-concurrent-trees/raw/main/Tisdall_Daniel_Designing_Concurrent_Trees_MSc_Thesis_Without_AppendixB.pdf)

## What is this?

In the spring of 2021 I wrote my master's thesis on designing _correct_ concurrent tree data structures. In particular, shared memory pointer based balanced trees.

## Abstract

> Concurrent tree data structures are difficult to design and implement correctly. This is due to numerous challenges at the design level and also at the implementation level. For example, at the design level, orderings of operations between processes on the graph structure must be correct. At the implementation level, programmers use fine grained shared memory operations to improve performance. As a result, they are forced to navigate complex interactions between hardware and programming language or library memory models.\
\
> As a result of the complexity, concurrent data structures are often found to exhibit correctness bugs and other violations of invariant properties, which can be extremely damaging, and expensive and difficult to fix. There is a need to attain strong assurances of correctness for such data structures, and many approaches have been tried.\
\
> In this thesis we present a methodology for improving the extent to which (concurrent) trees can be believed to be correct, using the TLA+ language and model checking. Model checking is an automatic verification technique that can efficiently explore large state spaces of possible program executions (including the instruction interleavings that can occur in a concurrent setting) to check whether certain properties are satisfied or violated. TLA+ is a flexible specification language, suited to modelling concurrent processes, which can be interpreted by model checkers, giving a complete history of the state of a model in case of a property violation.\
\
> The methodology we present is focused on pointer based concurrent tree data structures and can be used to check or track down complex bugs in existing structures, or to design and assure correctness of new structures. We applied our methodology, developing a new, verified, concurrent tree. We also applied the methodology to an existing state of the art concurrent tree from the literature, using it to find and explain critical correctness bugs.

## Code and future work

The code is currently private pending future work and time availability to create a release.

## Acknowledgements

I am very lucky to have had [Prof. Carlo A. Furia](https://bugcounting.net/) supervising me.
