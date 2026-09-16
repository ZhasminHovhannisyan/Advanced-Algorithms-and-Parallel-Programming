# Advanced Algorithms and Parallel Programming

Working repository for **Advanced Algorithms and Parallel Programming**, a Master's course at Politecnico di Milano (POLIMI), academic year **2026/27**, winter semester.

Lecture PDFs are edited in place. Earlier (clean) versions remain available through the git history of the same files.

## About the course

This course covers advanced topics in algorithm design and parallel programming. Students learn how a complex algorithm, including a parallel one, should be analyzed, designed, and assessed. The work moves from a theoretical formulation down to a real implementation, taking into account existing tools and real architectures, and where pitfalls appear in that transition.

The course is structured in two parts. The first part focuses on general methods and algorithms that are not usually covered by *Algoritmi e Principi dell’Informatica*, such as randomization, amortization, approximation algorithms, and string searching/matching. The second part deals with parallel programming: automatic vs. manual parallelization, parallelizing compilers, parallel patterns, partitioning (domain vs. functional decomposition), communication (cost, latency, bandwidth, visibility, synchronization), data dependencies, and tools/languages such as OpenMP and MPI. CUDA is not part of this edition of the course.

## Course objectives

- Analyze, design, and assess complex algorithms, including parallel ones.
- Apply methods that go beyond standard undergraduate algorithmics (randomization, amortization, approximation, string matching, and related techniques).
- Understand parallel machine models, parallel patterns, partitioning, communication, and data dependencies.
- Use real parallel programming tools and languages (POSIX threads, OpenMP, MPI, and related technologies) and compare them.
- Recognize implementation pitfalls when moving from theory to existing architectures and software stacks.



## Syllabus



### Part I — General methods and algorithms

**I-A**

1. Course objectives and introduction
2. Randomized algorithms: Las Vegas and Monte Carlo algorithms; analyzing randomized algorithms
3. Hiring problem and generating random permutations
4. Randomized Quicksort; worst-case analysis; average-case analysis
5. Order statistics; randomized divide-and-conquer
6. Primality test; fast exponentiation; secret key and cryptosystems

**I-B**

1. Karger’s min-cut algorithm; faster version by Karger and Stein
2. Randomized data structures: skip lists, treaps
3. Dynamic programming: memoization; examples including string matching and BDDs
4. Amortized analysis: dynamic tables; aggregate, accounting, and potential methods
5. Approximate programming
6. Competitive analysis; self-organizing lists; move-to-front heuristic



### Part II — Parallelization

1. Design of parallel algorithms; parallel algorithms and parallel programming
2. Parallel machine model
3. Parallel patterns: reduce, split, compact/expand, parallel prefix sum
4. Further parallel patterns: segmented scan, sort, map-reduce, kernel fusion
5. Optimizing parallel performance
6. Tools and languages: POSIX threads, OpenMP, Message Passing Interface (MPI)
7. Comparison of parallel programming technologies
8. Halide: high-performance image and array processing



## Repository structure

```
.
├── Lecture Slides/     lecture PDFs (annotated in place)
├── labs/               computer labs and projects (to be added)
├── LICENSE
└── README.md
```

- `Lecture Slides/` — current lecture handouts. Notes are written on these files; do not duplicate “clean” vs “annotated” copies. To recover a previous revision: `git log -- "Lecture Slides/<file>.pdf"` and check out the desired commit.
- `labs/` — reserved for exercise/computer-lab sessions and later project work (implementations, OpenMP/MPI code, notes). This directory will be added when the first lab material is committed.



## Teaching material and references

- T. Cormen, C. Leiserson, R. Rivest, and C. Stein, *Introduction to Algorithms*, MIT Press, 3rd edition, 2009. ISBN-13: 978-0262533058.
- R. Motwani and P. Raghavan, *Randomized Algorithms*, Cambridge University Press, 1995. ISBN-13: 978-0521474658.
- M. McCool, J. Reinders, and A. Robison, *Structured Parallel Programming: Patterns for Efficient Computation*, Morgan Kaufmann, 2012. ISBN: 0124159931. [http://parallelbook.com/](http://parallelbook.com/)
- P. Pacheco, *An Introduction to Parallel Programming*, Morgan Kaufmann, 1st edition, 2011. ISBN-13: 978-0123742605.



## License

All rights reserved. See `LICENSE`.

The license covers the entire repository (slides, notes, code, and documentation). Public visibility on GitHub is **not a grant of reuse**. Copying, redistribution, modification, commercial use, and reuse of the teaching materials are **not permitted**. Lecture slides and codes **remain copyright of their authors and Politecnico di Milano.**