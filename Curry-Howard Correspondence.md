>A powerful idea in modern type theory is the correspondence between propositions and types.

see also:
- [[Proof Verification]]

The correspondence between propositions and types, often called the "propositions as types" paradigm or the Curry-Howard correspondence, is a foundational concept in modern type theory and logic. This correspondence reveals a deep connection between logic, where we reason about propositions, and type theory, which deals with the categorization and manipulation of computational entities. It essentially equates proofs with programs and propositions with types, providing a bridge between formal logic and computer science.

### Foundations

The Curry-Howard correspondence was independently discovered by Haskell Curry and William Alvin Howard. Curry observed the analogy in combinatory logic, while Howard formalized it in the context of intuitionistic logic.

### The Core Ideas

- **Propositions as Types**: Under this correspondence, each logical proposition is associated with a type. The proposition being true corresponds to the type being inhabited, meaning there exists at least one term (or value) of that type. Conversely, a proposition being false corresponds to its type being uninhabited (having no terms).

- **Proofs as Programs**: A proof of a proposition is represented by a term (or program) of the corresponding type. Constructing a proof is thus akin to writing a program that inhabits a type. This concept is fundamental in proof assistants and functional programming languages, where writing a program to inhabit a type effectively proves a proposition.

### Mathematical Formulation

Let's consider a simple example to illustrate this concept mathematically. Suppose we have a proposition $A \implies B$ (if $A$ then $B$). In the propositions-as-types correspondence, this implication is represented by a function type $A \rightarrow B$. A proof of $A \implies B$ is then a function that takes a proof of $A$ (a term of type $A$) and returns a proof of $B$ (a term of type $B$).

For a concrete instance, let $A$ be the proposition "n is an even number", and $B$ the proposition "n squared is an even number". The proposition $A \implies B$ can be represented by a function that, given an even number $n$ (proof of $A$), returns $n^2$ (proof of $B$). The existence of this function (program) constitutes a proof that "if $n$ is even, then $n^2$ is even".

### Implications and Applications

- **[[Functional Programming]]**: The [[Curry-Howard correspondence]] has heavily influenced the design of functional programming languages like Haskell, where functions and types are the central constructs. It encourages writing correct-by-construction programs by closely tying the program logic to its type structure.

- **Proof Assistants**: Tools like Coq, Agda, and Lean exploit the Curry-Howard correspondence to verify mathematical proofs and software correctness. Users construct types corresponding to propositions they wish to prove and then write programs (proofs) inhabiting those types.

- **Homotopy Type Theory (HoTT)**: In extending the propositions-as-types correspondence, HoTT uses types to represent spaces rather than just propositions, allowing for a more nuanced exploration of equivalences and homotopies, further enriching the interplay between topology and logic.

The Curry-Howard correspondence underscores a powerful conceptual unity across disciplines, showing how constructing proofs, programming, and reasoning about types are interconnected activities guided by similar principles.