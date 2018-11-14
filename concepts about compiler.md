# concepts about compiler

标签（空格分隔）： compiler

---

**Lex** : break the source file into individual words,or tokens

**Parse** : Analyze the phrase structure of the program

**Semantic** **Actions** : build a piece of abstract syntax tree corresponding to each phrase

**Semantic** **Analysis** : determine what each phrase means relate uses of variables to their definitions  ,check types of expressions request translation of each phrase

**Frame** **Layout** : Place variables function-parameters etc into activation records(stack frames)in a machine-dependent way

**Translate** : Produce *intermediate representation trees*(**IR trees**),a notation that is not tied to any particular source language or target-machine arcitecture

**Canonicalize** : Hoist side effects out of expressions,and clean up conditional branches, for the convenience of the next phases

**Instruction Selection** : Group the IR-tree nodes into clumps that correspond to the actions of target-machine instructions

**Control Flow Analysis** : Analyze the sequence of instructions into a control flow graph that shows all the possible flows of control the program might fllow when it executes

**Dataflow Analysis** : Gather information about the flow of information through variables of the program;for example,liveness analysis calculates the places where each program variable holds a still-needed value(is live)

**Register Allocation** : Choose a register to hold each of the variables and temporary values used by the program variables not live at the same time can share the same register

**Code Emission** : Replace the temporary names in each machine instruction with machine registers

**useful abstractions** : *context-free grammars* for parsing
*regular expressions* for lexical analysis

**DFA deterministic finite automaton**




