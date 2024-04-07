see also:


Type theory is a rich and complex field that spans mathematics, [[logic]], and computer science. It provides a framework for defining, manipulating, and reasoning about different kinds of entities, often called "types". In essence, type theory is concerned with categorizing objects (which can be anything from simple numbers to complex data structures or even functions) into various types, and defining operations that can be performed on these types. This helps in ensuring correctness in mathematical proofs and programming languages by preventing operations that do not make sense from a type perspective (e.g., "adding" a number to a string).

### Origins and Motivation

Type theory originated with [[Bertrand Russell]]'s early 20th-century efforts to resolve the paradoxes in [[set theory]], notably [[Russell's Paradox]]. Russell introduced a hierarchical system of types to prevent self-referential sets, laying the groundwork for what would evolve into modern type theories.

### Basic Concepts

At its core, type theory introduces several key concepts:

- **Types**: A type can be thought of as a collection of entities that share some common property. For instance, the type "integer" includes all integer numbers.

- **Terms**: These are the basic objects of type theory. A term can be a simple object (like the number $3$) or a more complex expression (like a function). Each term has a type.

- **Type Judgements**: These are statements that assign a term to a type, often denoted as $term : type$, indicating that the term belongs to the specified type.

- **Functions and [[Lambda Calculus]]**: Functions are mappings from terms of one type to terms of another type. The lambda calculus provides a formalism for defining and using functions within type theory.

- **[[Curry-Howard Correspondence|Propositions as Types]]**: A powerful idea in modern type theory is the correspondence between propositions and types. Under this view, proving a proposition corresponds to finding a term of a certain type.

### Major Variants of Type Theory

- **[[Simple Type Theory]]**: This is the basic form of type theory, where types are not allowed to depend on terms. It provides a foundation for functional programming languages and formal logic.

- **[[Dependent Type Theory]]**: In dependent type theory, types can depend on terms. This allows for more expressive power in defining and proving properties of mathematical constructs and programs. It serves as the basis for proof assistants like Coq and Agda.

- **[[Homotopy Type Theory]] (HoTT)**: A more recent development that interprets types as spaces and type equivalences as paths between spaces. It provides a new foundation for mathematics with connections to topology.

### Mathematical Formalism

To understand type theory from a mathematical perspective, consider the concept of a function in simple type theory. A function $f$ from type $A$ to type $B$ can be represented as $f: A \rightarrow B$. This means for every term $x$ of type $A$, $f(x)$ is a term of type $B$. The lambda calculus notation for such a function might be $\lambda x:A. f(x)$, where $\lambda$ signifies a function definition, $x:A$ denotes that $x$ is of type $A$, and $f(x)$ is the function's body.

In dependent type theory, the type of the output can depend on the actual input term, not just its type. For instance, a function $g$ might have a type $g: \forall (x:A), B(x)$, where $B(x)$ is a type that depends on the term $x$. This allows for much more precise type definitions and is a cornerstone of proofs involving complex mathematical structures.

Type theory's richness and depth make it an essential tool in both theoretical and applied domains, including software development, where it helps in ensuring program correctness and safety.

