To be distinguished from: [[Complexity Theory]]

Complexity theory is a foundational pillar of computer science and mathematics that focuses on classifying computational problems according to their inherent difficulty, and the resources required to solve them. At the heart of complexity theory lies the notion of computational problems and the models of computation used to solve them, such as Turing machines, Boolean circuits, and quantum computers. The field intricately explores the limits of what can be computed in a reasonable amount of time and space, and it distinguishes between problems that are solvable with feasible resources from those that are not.

### Key Concepts and Classes

1. **Computational Problems**: These are tasks or questions with a precise statement of the input and a method for determining whether a given input satisfies the conditions of the problem. Problems can be decision problems (yes/no answers), optimization problems, counting problems, etc.

2. **Decision Problems and Languages**: A decision problem can be represented as a language $L$, where $L$ is a set of strings over some alphabet. The problem is to decide, for any given string $s$, whether $s \in L$.

3. **[[Complexity Classes]]**: These are sets of problems classified according to the resources (time, space) required for their solution on certain computational models. The most well-known classes include:
   - **P**: Problems solvable in polynomial time by a deterministic Turing machine. That is, there exists an algorithm that solves any problem instance of size $n$ in $O(n^k)$ time for some constant $k$.
   - **NP**: Problems for which a "yes" solution can be verified in polynomial time by a deterministic Turing machine. Formally, a problem is in NP if there exists a polynomial-time verifier for the problem.
   - **PSPACE**: Problems solvable with polynomial amount of space, regardless of the time it takes.
   - **EXP**: Problems solvable in exponential time. More formally, problems that can be solved in $O(2^{p(n)})$ time for some polynomial $p(n)$.
   - **NP-complete**: A subset of NP that are as hard as the hardest problems in NP. If any NP-complete problem can be solved in polynomial time, then $P = NP$.
   - **NP-hard**: Problems that are at least as hard as the hardest problems in NP, but not necessarily in NP (i.e., they may not have a polynomial time verifier).

4. **$P$ vs $NP$ Problem**: This is one of the most fundamental open questions in computer science. It asks whether every problem whose solution can be quickly verified by a deterministic Turing machine can also be quickly solved by a deterministic Turing machine. Formally, it asks whether $P = NP$.

5. **Turing Machines and Complexity**: A Turing machine is a theoretical computing machine invented by Alan Turing. It's used as a model of computation to define the complexity classes. A deterministic Turing machine (DTM) operates in a deterministic manner, whereas a non-deterministic Turing machine (NTM) can explore multiple branches of computation simultaneously, which is crucial for the definition of NP.

6. **Reductions and Hardness**: A problem $A$ is reducible to another problem $B$ if an algorithm for solving $B$ efficiently (usually in polynomial time) can be used to solve $A$ efficiently. This concept is central to proving NP-completeness and NP-hardness, where a problem is shown to be NP-complete by reducing a known NP-complete problem to it.

### Important Results and Theorems

- **Cook-Levin Theorem**: This theorem states that the Boolean satisfiability problem (SAT) is NP-complete, establishing the first problem known to be NP-complete and paving the way for demonstrating the NP-completeness of many other problems.
  
- **Savitch's Theorem**: It shows that deterministic and non-deterministic space complexities are closely related: $NSPACE(s(n)) \subseteq DSPACE(s(n)^2)$, implying that nondeterministic space complexities can be simulated by deterministic space complexities with at most a quadratic blowup.

- **Time-Space Tradeoffs**: These are results that show how the time complexity of solving a problem varies with the amount of memory space available, and vice versa.

Complexity theory continues to evolve, exploring new models of computation, such as quantum computing, and extending its reach to other disciplines, including cryptography, quantum information theory, and algorithmic game theory. The field remains vibrant with many open problems and a dynamic landscape of theoretical advancements.