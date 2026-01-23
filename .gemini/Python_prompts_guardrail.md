Python Prompts Guardrail — Mastery Curriculum
Purpose: This document is a comprehensive curriculum execution ledger used by Python_Learning_Guardrail_Co-Pilot.Key Features:
Each prompt fully exhausts its topic(s) conceptually, practically, and diagnostically, with expanded subtopics for depth equivalent to a bootcamp + university-level course.
Includes detailed breakdowns of concepts like string operations, file handling, encapsulation, and more to ensure no gaps in understanding.
Teaching depth emphasizes first principles, mental models, real-world applications, common pitfalls, and advanced nuances.
Executed strictly in order and gated by Proceed.


EXECUTION RULES (NON-NEGOTIABLE)

The agent may ONLY teach the currently active prompt.
Every concept must be explained from first principles.
Each prompt MUST include:
Conceptual theory and mental models
Python syntax and semantics with code examples
Common mistakes, debugging strategies, and error handling
Real-world analogies and applications
Exercises with variations and edge cases
Project integration with iterative refinements

Every prompt modifies the same evolving project.
Advancement requires explicit learner evaluation via Proceed, assessing depth of understanding through discussions, code reviews, and reflections.


STAGE 1 — BEGINNER: LEARN THE BASICS
Prompt 01 — Basic Syntax and What Programming Is
Teaching Scope
Explain what programming means, how humans instruct machines, basic Python syntax rules, whitespace significance, and how Python executes code (top-to-bottom). Cover the role of Python in backend, data science, automation, AI/ML, and its hybrid paradigm nature.
Concepts to Exhaust

Source code vs execution (human-readable text vs machine instructions)
Interpreter loop (REPL vs script execution)
Statements vs expressions (actions vs values)
Indentation blocks (scope definition, common indentation errors)
Why errors stop execution (sequential flow, traceback analysis)
Comments as non-executable metadata (single-line #, multi-line """)
Python's interpreted nature vs compiled languages
Variable scope introduction (global vs local teaser)
Clean code principles from the start (readability, PEP 8 basics)

Demonstrations

Minimal print() program with variations (print with sep, end)
Correct vs incorrect indentation examples leading to IndentationError
Execution order experiment with multiple prints and simple operations

Exercise
Write a Python script that prints a welcome message, the project name, and a confirmation showing execution order. Experiment with indentation and comments; debug any errors.
Project Integration
Create main.py as the permanent project entry point, adding initial comments and a basic print statement for setup verification.
Evaluation Criteria

Correct execution and ordering
No syntax errors, proper indentation
Understanding of error stopping and basic debugging


Prompt 02 — Variables and Data Types
Teaching Scope
Explain variables as references to objects in memory, primitive data types, mutability, and immutability. Dive deep into each type, especially strings with operations and methods.
Concepts to Exhaust

Assignment vs equality (= vs ==)
Naming conventions (snake_case, constants, reserved words)
Primitive types: int (arbitrary precision), float (precision limits, NaN/inf), str (immutability, Unicode), bool (True/False, truthy/falsy values)
type() and id() inspection (object identity)
Runtime type errors (TypeError examples)
Mutability vs immutability (why strings are immutable, lists mutable)
String specifics: escaping (\n, \t, \), methods (upper, lower, strip, split, join, find, replace), indexing/slicing, formatting (% , .format, f-strings), raw strings (r""), multi-line strings (""")
Working with strings: concatenation (+, *), interpolation, common pitfalls (mutable default args teaser)
NoneType and its uses

Demonstrations

Variable reassignment and id changes for mutables/immutables
Arithmetic with mixed types (int + float promotion)
String operations: slicing, formatting examples with variables

Exercise
Declare variables for application name (str), version (float), author (str), active (bool); print them formatted using f-strings. Manipulate a string: split a sentence, join words, handle escapes.
Project Integration
Introduce a configuration section in main.py with typed variables, including string processing for a welcome message.
Evaluation Criteria

Valid variable usage and naming
Correct data type handling, including string methods and mutability demos
Error-free operations on types


Prompt 03 — Conditionals
Teaching Scope
Explain decision-making using boolean logic and conditional execution, including nested logic and real-world decision trees.
Concepts to Exhaust

Truth tables for and, or, not
Comparison operators (==, !=, >, <, >=, <=, is, in)
if/elif/else flow control, including else clause usage
Logical operators (short-circuit evaluation: and/or laziness)
Truthy/falsy values (0, "", [], None as falsey)
Nested conditionals and flattening with guards
Common logic errors (off-by-one, misplaced else)
Conditional expressions (ternary: a if cond else b)

Demonstrations

Nested conditionals for multi-level decisions
Short-circuit examples (e.g., x and x.method() avoiding AttributeError)

Exercise
Build conditional responses based on user input (e.g., age check with multiple branches). Use ternary for simple cases.
Project Integration
Add logic to control execution paths in main.py, like config validation with conditionals.
Evaluation Criteria

Accurate conditional logic with short-circuiting
Handling of edge cases (falsy values, nested logic)
No redundant checks


Prompt 04 — Loops
Teaching Scope
Explain iteration, counters, and repetition models, with emphasis on efficiency and common patterns.
Concepts to Exhaust

for loops (over iterables, range, enumerate, zip)
while loops (condition-based, sentinel values)
Infinite loops and prevention
break, continue, else (no-break detection)
Loop invariants and proofs (conceptual)
Nested loops and complexity (O(n^2) intro)
Common patterns: accumulation, filtering, searching

Demonstrations

Iterating over ranges, lists, strings with enumerate/zip
Debugging loop errors (off-by-one, infinite)

Exercise
Process a collection repeatedly with loops: sum numbers, find max, filter evens. Use nested for matrix traversal.
Project Integration
Automate repetitive tasks in the project, like processing config lists.
Evaluation Criteria

Correct loop termination and invariants
Efficient iteration with built-ins (no manual indexing if unnecessary)
Handling nested loops


Prompt 05 — Type Casting
Teaching Scope
Explain implicit vs explicit type conversion and why types matter, with safe practices and error handling.
Concepts to Exhaust

Implicit coercion (e.g., int + float -> float)
Explicit casting functions (int(), float(), str(), bool(), list(), tuple(), set(), dict())
Casting failures and errors (ValueError on invalid str to int)
Type compatibility and conversions (str to list, ord/char)
Safe casting with try-except or checks (isdigit, etc.)
Advanced: custom casting with classes (teaser)

Demonstrations

Converting user input safely (input() -> int with validation)
Mixed-type operations leading to TypeError

Exercise
Safely convert numeric input and perform calculations; convert list to set for uniqueness.
Project Integration
Validate and cast configuration values in main.py.
Evaluation Criteria

Safe type conversions with error handling
Error-free casting across types
Understanding implicit risks


Prompt 06 — Exceptions
Teaching Scope
Explain failure handling and defensive programming, including custom exceptions and best practices.
Concepts to Exhaust

Built-in error types (SyntaxError, ValueError, TypeError, IndexError, KeyError, AttributeError, ZeroDivisionError, etc.)
Error propagation and stack traces
try/except/else/finally blocks (else for no-exception, finally for cleanup)
Raising exceptions (raise ValueError("msg"))
Custom exception classes (inheritance from Exception)
Exception chaining (raise NewExc from OldExc)
Assertions (assert cond, "msg") for debugging
Common patterns: retry logic, logging errors

Demonstrations

Handling invalid input with specific except blocks
Creating and raising custom exceptions

Exercise
Safely handle invalid inputs with try-except; raise custom exception on bad config.
Project Integration
Stabilize runtime in main.py with exception guards.
Evaluation Criteria

Proper exception handling hierarchy (specific to broad)
Graceful error recovery and custom raises
Use of finally for resources


Prompt 07 — Functions and Builtin Functions
Teaching Scope
Explain abstraction, reuse, and built-in functions, with deep dive into parameters, scope, and functional patterns.
Concepts to Exhaust

Function definition (def, docstrings)
Parameters: positional, keyword, defaults, *args, **kwargs, annotations (type hints teaser)
Return values (multiple returns, None default)
Scope: local, global, nonlocal (in nested funcs)
Built-ins: len(), sum(), max(), min(), sorted(), map(), filter(), any(), all(), zip(), enumerate()
Function composition and higher-order functions (functions as args/returns)
Recursion teaser (base case importance)
Common mistakes: mutable defaults, global overuse
Variable scope in depth (LEGB rule: Local, Enclosing, Global, Built-in)

Demonstrations

Refactoring code into functions with *args/**kwargs
Variable scope issues (global modification, nonlocal in closures)

Exercise
Refactor logic into reusable functions; use built-ins to process lists.
Project Integration
Modularize the codebase with functions for config handling.
Evaluation Criteria

Correct function definitions with advanced params
Proper scoping (no global abuse)
Effective use of built-ins


Prompt 08 — Lists, Tuples, Sets
Teaching Scope
Explain grouped data storage and core collections, with operations, complexities, and use cases.
Concepts to Exhaust

Lists: mutability, indexing/slicing, methods (append, extend, insert, remove, pop, sort, reverse, index, count, clear)
Tuples: immutability, packing/unpacking, namedtuples (collections)
Sets: unordered, unique, mutability, operations (add, remove, discard, pop, clear, union |, intersection &, difference -, symmetric_difference ^, issubset, issuperset)
Membership testing (in/not in O(1) for sets)
List vs tuple vs set trade-offs (performance, use cases: lists for ordered, tuples for fixed, sets for unique/fast lookup)
Nested collections (list of lists)
Common mistakes: modifying during iteration, aliasing

Demonstrations

List modifications and slicing idioms (copy with [:])
Set operations for data deduplication

Exercise
Manipulate lists, tuples, and sets: sort list, unpack tuple, compute set intersections.
Project Integration
Store structured records, like config lists or unique items.
Evaluation Criteria

Correct collection usage and methods
Understanding mutability and operations
Efficient membership checks


Prompt 09 — Dictionaries
Teaching Scope
Explain key-value models and structured mapping, with hashing and advanced features.
Concepts to Exhaust

Hashing concepts (hashable keys: immutables only)
Access patterns: get(default), items(), keys(), values(), pop(key, default), update(), setdefault()
Dictionary comprehensions {k:v for ...}
Nested dictionaries and defaultdict (collections)
OrderedDict (preserving insertion order, since 3.7 dicts are ordered)
Common mistakes: mutable keys, KeyError avoidance
Use cases: configs, counters, graphs

Demonstrations

Building and querying dictionaries with get/setdefault
Handling missing keys safely

Exercise
Create and query dictionaries for data; use comprehension for transformation.
Project Integration
Use dictionaries for configuration mapping in main.py.
Evaluation Criteria

Efficient key-value operations and comprehensions
Error handling for keys (no KeyError)
Understanding ordering and hashing


Prompt 10 — File Handling and I/O
Teaching Scope
Explain filesystem interaction, persistence, and I/O operations, including text/binary modes and best practices.
Concepts to Exhaust

File modes (r, w, a, r+, w+, binary b)
Context managers (with open for auto-close)
Reading: read(), readline(), readlines(), iterable file
Writing: write(), writelines()
Seeking/telling (seek, tell)
Path handling (os.path, pathlib for modern)
Serialization basics (json.dump/load, pickle for objects)
Common errors: FileNotFound, PermissionError, encoding (UTF-8 default)
CSV/JSON handling (csv module, json)

Demonstrations

Reading/writing text files with with-block
JSON serialization for configs

Exercise
Read from a file, process lines, write output; handle JSON data.
Project Integration
Add persistent storage for project state (e.g., save/load config).
Evaluation Criteria

Safe file operations with context managers
Proper encoding and mode usage
Error handling for I/O


STAGE 2 — INTERMEDIATE: DATA STRUCTURES & ALGORITHMS
Prompt 11 — Data Structures & Algorithms: Arrays and Linked Lists
Teaching Scope
Explain linear data structures and their implementations, with time/space complexities.
Concepts to Exhaust

Arrays (Python lists: dynamic arrays, amortized O(1) append)
Linked lists: singly/doubly linked (custom Node class, head/tail)
Operations: access (O(1) array, O(n) list), insert/delete (O(1) list head, O(n) array)
Use cases: arrays for random access, lists for frequent inserts/deletes
Collections.deque for efficient queues/stacks

Demonstrations

Implementing a simple linked list class with add/remove
Comparing list vs deque performance

Exercise
Build a linked list and perform operations; convert to deque for efficiency.
Project Integration
Incorporate a linked list or deque for dynamic data in project.
Evaluation Criteria

Correct implementation of nodes and operations
Understanding trade-offs (time/space)
No memory leaks in custom impl


Prompt 12 — Heaps, Stacks, and Queues
Teaching Scope
Explain priority and ordered structures, with implementations.
Concepts to Exhaust

Stacks (LIFO): list as stack (append/pop), use cases (undo, recursion sim)
Queues (FIFO): deque (append/popleft), queue module for threads
Heaps: heapq (min-heap, heappush/heappop, heapify), max-heap simulation (-x)
Priority queues (heapq with tuples)
Complexities: O(1) stack/queue ops, O(log n) heap

Demonstrations

Using deque for queues, heapq for priorities
Heap operations for sorting (heapsort)

Exercise
Implement stack and queue; use heap for priority tasks.
Project Integration
Add undo/redo using stacks, task queue.
Evaluation Criteria

Proper order enforcement (LIFO/FIFO)
Efficient operations with correct complexities
Heap usage for priorities


Prompt 13 — Hash Tables
Teaching Scope
Explain hashing for fast lookups, with custom simulation.
Concepts to Exhaust

Hash functions (hash() in Python, collisions)
Collision resolution (chaining, open addressing)
Dictionaries as hash tables (O(1) average lookup)
Load factor and resizing
Custom hash table impl (list of lists for chaining)

Demonstrations

Custom hash table simulation with add/get
Performance benefits over lists

Exercise
Simulate a hash table with collision handling.
Project Integration
Optimize lookups in project data using dicts.
Evaluation Criteria

Handling collisions correctly
Fast access demonstration (O(1))
Understanding resizing


Prompt 14 — Binary Search Tree
Teaching Scope
Explain tree structures for sorted data, with balancing intro.
Concepts to Exhaust

Nodes (value, left, right), traversal (in-order, pre-order, post-order, level-order)
Insertion, deletion, search (O(log n) balanced)
Balanced vs unbalanced (degenerate to list O(n))
AVL/self-balancing teaser (not impl)
BST properties (left < root < right)

Demonstrations

Implementing a BST class with recursive insert/search
Traversal methods (recursive/iterative)

Exercise
Build and traverse a BST; insert/delete nodes.
Project Integration
Use BST for sorted storage in project.
Evaluation Criteria

Correct tree operations and properties
Balanced understanding (avoid degeneration)
Proper traversals


Prompt 15 — Recursion
Teaching Scope
Explain recursive thinking, base cases, and optimization.
Concepts to Exhaust

Stack frames and call stack
Recursion depth limits (sys.getrecursionlimit)
Tail recursion and optimization (Python lacks, but conceptual)
Memoization (lru_cache decorator teaser)
Divide-and-conquer patterns
Common recursions: factorial, Fibonacci, tree traversal, merge sort

Demonstrations

Factorial, Fibonacci with/without memo
Recursive tree traversal

Exercise
Solve problems recursively: factorial, file tree walk.
Project Integration
Add recursive data processing (e.g., nested config).
Evaluation Criteria

Proper base cases and termination
Avoiding stack overflow (depth awareness)
Memo for efficiency


Prompt 16 — Sorting Algorithms
Teaching Scope
Explain sorting techniques, efficiencies, and implementations.
Concepts to Exhaust

Comparison sorts: bubble (O(n^2)), insertion (O(n^2) adaptive), selection (O(n^2))
Efficient: merge (O(n log n), divide-conquer), quick (O(n log n) avg, partition), heap (O(n log n))
Non-comparison: counting, radix (for ints/strings)
Time/space complexities, stable vs unstable (merge stable, quick not)
Python's sorted() (Timsort: merge+insertion hybrid)

Demonstrations

Implementing merge sort recursively
Comparing efficiencies with timeit

Exercise
Implement and test bubble, merge, quicksort; use sorted() with keys.
Project Integration
Sort project data collections with custom keys.
Evaluation Criteria

Correct sorting implementations
Complexity awareness and stability
Choice of algo based on data


STAGE 3 — ADVANCED: MODULES, PARADIGMS, AND TOOLS
Prompt 17 — Modules (Builtin and Custom)
Teaching Scope
Explain modularity for scale and organization, with packaging.
Concepts to Exhaust

Builtin modules: math (trig, constants), random (choice, shuffle), os (path, environ), sys (argv, path)
Custom modules: import, from ... import, aliases (as)
__init__.py for packages, submodules
Absolute vs relative imports (from . import)
Module search path (sys.path, PYTHONPATH)
Namespaces and __name__ == "__main__"
Common mistakes: circular imports, shadowing builtins

Demonstrations

Splitting code into modules, importing
Package creation with init

Exercise
Refactor project into modules; use builtin for math ops.
Project Integration
Introduce /core and /utils modules/subpackages.
Evaluation Criteria

Clean imports without cycles
Proper package structure
Effective use of builtins


Prompt 18 — Lambdas
Teaching Scope
Explain anonymous functions for concise code, with functional style.
Concepts to Exhaust

Lambda syntax (lambda args: expr)
Use in sorting (key=lambda x: x[1]), map/filter/reduce (functools.reduce)
Limitations (single expr, no statements, no annotations)
Closures (capturing variables)
Higher-order functions
Common pitfalls: late binding in loops

Demonstrations

Lambda in sorted() with multi-keys
Closures with lambdas in list comps

Exercise
Use lambdas in functional operations: map to square, filter evens.
Project Integration
Simplify callbacks and sorts in project.
Evaluation Criteria

Appropriate lambda usage without overuse
Readability in functional chains
Closure handling


Prompt 19 — Decorators
Teaching Scope
Explain function wrappers for behavior modification, with advanced uses.
Concepts to Exhaust

Decorator syntax (@decorator)
Writing decorators (def wrapper(func): return inner)
With arguments (@decorator(arg))
functools.wraps for metadata preservation
Class decorators, method decorators
Use cases: timing, logging, memoization, auth
Chaining multiple decorators

Demonstrations

Timing decorator with time.perf_counter
Memoization (custom or lru_cache)

Exercise
Create and apply timing/logging decorators.
Project Integration
Add logging/timing to project functions.
Evaluation Criteria

Correct wrapping and args handling
Preserved metadata with wraps
Chained decorators


Prompt 20 — Iterators
Teaching Scope
Explain iterable protocols and custom iteration, with generators.
Concepts to Exhaust

Iterable vs iterator (iter() returns iterator)
__iter__ and __next__ protocol
StopIteration to end
Itertools: count, cycle, repeat, product, permutations, combinations, chain, islice, tee
Infinite iterators and handling
Custom iterator classes

Demonstrations

Custom iterator for range-like
Infinite with takewhile

Exercise
Implement a custom iterator for project data.
Project Integration
Custom data iteration in project (e.g., lazy loading).
Evaluation Criteria

Proper protocol implementation
Memory efficiency with iterators
Use of itertools


Prompt 21 — Regular Expressions
Teaching Scope
Explain pattern matching for text processing, with advanced patterns.
Concepts to Exhaust

re module: compile, match (start), search, findall, finditer, sub, split
Patterns: quantifiers (*, +, ?, {n,m}), groups (()), non-capturing (?:), lookaheads/behinds (?=, ?!, ?<=, ?<!)
Flags (re.IGNORECASE, re.MULTILINE, re.DOTALL)
Compilation for efficiency (re.compile)
Common use: validation (email, phone), extraction, sanitization
Pitfalls: greedy vs non-greedy (.* vs .*?), backtracking

Demonstrations

Email validation regex
Group extraction and substitution

Exercise
Validate and extract with regex (e.g., parse log lines).
Project Integration
Add input validation layer with re.
Evaluation Criteria

Accurate, efficient patterns
Handling groups and flags
Non-greedy matching


Prompt 22 — Object-Oriented Programming: Classes and Inheritance
Teaching Scope
Explain OOP principles, class design, and encapsulation.
Concepts to Exhaust

Classes as blueprints (def class, self)
Attributes: instance (self.x), class (shared)
Encapsulation: private (_x, __x name mangling), properties (@property, @setter)
Inheritance: single/multiple (class Child(Parent)), method resolution order (mro())
super() for parent calls
Polymorphism (duck typing, same method names)
Abstract base classes (abc module, ABCMeta, abstractmethod)
Composition vs inheritance (favor composition)

Demonstrations

Class hierarchies with inheritance
Property for controlled access

Exercise
Design classes with inheritance and properties.
Project Integration
Introduce primary project classes with encapsulation.
Evaluation Criteria

Proper encapsulation and private attrs
Reuse via inheritance/composition
MRO understanding in multiple inherit


Prompt 23 — Methods and Dunder Methods
Teaching Scope
Explain special methods for customization and operator overloading.
Concepts to Exhaust

Instance methods (self), class methods (@classmethod, cls), static methods (@staticmethod)
Dunder methods: init (constructor), del (destructor), str/repr (string reps), eq/ne (comparison), hash (for dict keys), call (callable objects)
Operator overloading: add, sub, mul, lt, etc.
new vs init (advanced creation)
Slots (slots) for memory optimization

Demonstrations

Custom string representation and equality
Operator overloading for vector class

Exercise
Implement dunder methods for custom class.
Project Integration
Enhance project classes with operators and callables.
Evaluation Criteria

Correct method types (instance/class/static)
Proper dunder for built-in behaviors
Overloading for intuitive use


Prompt 24 — Package Managers (PyPI, Pip, Conda, Poetry, pdm, uv)
Teaching Scope
Explain dependency management tools, with reproducibility focus.
Concepts to Exhaust

PyPI repository (publishing packages)
Pip: install, uninstall, list, freeze > requirements.txt, --user, --editable
Conda: envs with non-Py deps (e.g., scientific)
Poetry: pyproject.toml declarative, virtualenv auto, add/remove
pdm: modern, fast, pyproject-based
uv: ultra-fast pip alternative
Lock files (Pipfile.lock, poetry.lock)
Conflicts resolution, version specifiers (~=, ==, >=)

Demonstrations

Installing packages with pip/poetry
requirements.txt vs pyproject.toml

Exercise
Set up dependencies for project using Poetry.
Project Integration
Add external packages with lock file.
Evaluation Criteria

Reproducible setup with lock
Conflict resolution
Tool choice rationale


Prompt 25 — Common Packages
Teaching Scope
Introduce essential third-party packages, selected based on roadmap goals (backend, data, etc.).
Concepts to Exhaust

Requests: HTTP (get/post, headers, params, json, sessions, auth)
NumPy: arrays, vector ops, broadcasting, linalg
Pandas: DataFrames, series, read_csv/excel, groupby, merge, pivot
Selection: based on path (e.g., TensorFlow for ML, but focus core)
Installation and basic usage
Best practices: virtualenvs for isolation

Demonstrations

Fetching data with requests
Basic data manipulation with Pandas

Exercise
Integrate requests for API call; use Pandas for data.
Project Integration
Enhance project with libs (e.g., load external data).
Evaluation Criteria

Proper integration and usage
Understanding package ecosystems
Error handling in libs


Prompt 26 — Configuration (pyproject.toml)
Teaching Scope
Explain project configuration standards, with tool integrations.
Concepts to Exhaust

TOML format (tables, arrays, strings)
Sections: [tool.poetry] for deps, [build-system], [tool.black] for formatters, [tool.pytest] for tests
Vs setup.py (legacy), requirements.txt
Reading config in code (tomllib in 3.11+, toml package)
Dynamic configs (os.environ override)

Demonstrations

Configuring tools like black, pytest
Parsing pyproject.toml in script

Exercise
Create pyproject.toml for project with deps and tools.
Project Integration
Standardize config, read in main.py.
Evaluation Criteria

Valid TOML syntax
Tool integration (e.g., poetry deps)
Runtime config loading


Prompt 27 — List Comprehensions and Generator Expressions
Teaching Scope
Explain concise data transformations, with performance considerations.
Concepts to Exhaust

List comp: [expr for item in iter if cond]
Set/dict comps: {expr}, {k:v}
Generator expressions: (expr for ...) lazy
Nested comprehensions (flattening with double for)
Walrus operator (:=) in comps (3.8+)
Memory usage: lists eager vs gens lazy
Common pitfalls: leaking vars, over-nesting

Demonstrations

Filtering/mapping with comps
Memory comparison with sys.getsizeof

Exercise
Refactor loops to comprehensions; use gen for large data.
Project Integration
Simplify data processing in project.
Evaluation Criteria

Readability in comps
Efficiency with gens
Nested handling


Prompt 28 — Paradigms: Context Manager
Teaching Scope
Explain resource management paradigms, with custom impl.
Concepts to Exhaust

with statement for enter/exit
__enter__ (setup, return self), __exit__ (cleanup, handle exc)
contextlib: @contextmanager (yield), suppress, redirect_stdout
Use cases: files, locks, temp changes (os.chdir)
Async context managers (3.7+: aenter/aexit)

Demonstrations

File handling with context
Custom manager for timing

Exercise
Implement a context manager for project resource.
Project Integration
Manage resources safely (e.g., db conn).
Evaluation Criteria

Proper cleanup in exit
Exception handling (suppress or propagate)
Yield usage in @contextmanager


Prompt 29 — Learn a Framework
Teaching Scope
Explain web frameworks and choices, with basic app building.
Concepts to Exhaust

Synchronous: Pyramid (configurable), Plotly Dash (data viz apps)
Asynchronous: gevent (greenlets), aiohttp (async HTTP), Tornado (non-blocking), Sanic (fast async)
Sync+Async: FastAPI (modern, auto-docs, type hints), Django (batteries-included, ORM), Flask (minimal, extensions)
Core: routing, templates (Jinja), requests/responses, middleware, APIs (REST, async)
Deployment basics (gunicorn, uvicorn)
Trade-offs: speed (async), ease (Django), flexibility (Flask)

Demonstrations

Basic app in Flask/FastAPI with routes
Handling GET/POST, JSON

Exercise
Build a simple web app with endpoints.
Project Integration
Add web interface to project.
Evaluation Criteria

Functional app with routes
Framework understanding (sync vs async)
Basic security (input validation)


Prompt 30 — Concurrency: Multiprocessing, Asynchrony, GIL, Threading
Teaching Scope
Explain parallel execution models, with GIL limitations.
Concepts to Exhaust

GIL (Global Interpreter Lock: one thread executes Python at a time)
Threading: for I/O-bound (threading.Thread, Lock, RLock, Queue), race conditions, daemon
Multiprocessing: for CPU-bound (Process, Pool, shared mem with Manager, Queue)
Asynchrony: asyncio (event loop, async def, await, coroutines, tasks, gather, as_completed)
uvloop for faster asyncio
Hybrid: concurrent.futures (ThreadPoolExecutor, ProcessPoolExecutor)
Common issues: deadlocks, shared state, context switching

Demonstrations

Threaded vs process pools for downloads/computes
Async functions for I/O (aiohttp)

Exercise
Parallelize tasks: multi-thread download, async API calls.
Project Integration
Optimize performance (e.g., async data fetch).
Evaluation Criteria

Correct model choice (I/O thread, CPU process, async)
Race condition avoidance (locks, queues)
Efficient async patterns


Prompt 31 — Environments (Pipenv, virtualenv, pyenv)
Teaching Scope
Explain isolation and version management, with multi-version handling.
Concepts to Exhaust

virtualenv: creation (virtualenv env), activate/deactivate, --system-site-packages
Pipenv: deps+env (Pipfile, install, shell), scripts
pyenv: Python version manager (install versions, global/local, shims)
venv module (built-in virtualenv)
Common workflows: pyenv + virtualenv/poetry
Isolation benefits: dep conflicts, reproducibility

Demonstrations

Activating environments, installing in isolation
Managing multiple Python versions with pyenv

Exercise
Set up project environment with pyenv and poetry.
Project Integration
Ensure reproducibility with env setup.
Evaluation Criteria

Isolated setup without global pollution
Version control with pyenv
Script activation


Prompt 32 — Static Typing (typing, mypy, pyright, pyre, Pydantic)
Teaching Scope
Explain type safety and annotations, with validation.
Concepts to Exhaust

Type hints: annotations (def f(x: int) -> str), typing (List, Dict, Union, Optional, Any, TypeVar)
Checkers: mypy (static), pyright (VSCode), pyre (Facebook), config files
Pydantic: data validation (BaseModel, fields, validators, parse_obj)
Runtime checks (typeguard) vs static
Gradual typing, stubs (.pyi)
Benefits: catch errors early, IDE help

Demonstrations

Annotating functions/classes
Running mypy on code

Exercise
Add types to project; use Pydantic for config validation.
Project Integration
Improve maintainability with hints.
Evaluation Criteria

Type correctness and generics
Validation with Pydantic
Passing static checks


Prompt 33 — Code Formatting (yapf, black, ruff)
Teaching Scope
Explain style enforcement, with linters and formatters.
Concepts to Exhaust

Formatters: black (opinionated, auto), yapf (configurable, Google/PEP8)
Linters: ruff (fast, replaces flake8/pylint/isort, rules config)
Config: pyproject.toml [tool.black], .ruff.toml
Pre-commit hooks for auto-format
PEP 8/257 standards (line length, imports, naming)

Demonstrations

Formatting code with black
Fixing lint issues with ruff --fix

Exercise
Format and lint project code.
Project Integration
Standardize code quality with hooks.
Evaluation Criteria

Consistent style per config
No lint errors/warnings
Auto-fix integration


Prompt 34 — Documentation (Sphinx)
Teaching Scope
Explain professional docs, with auto-generation.
Concepts to Exhaust

Docstrings: reST format ("""doc"""), Google/Numpy styles
Sphinx: conf.py, rst files, extensions (autodoc, napoleon, myst)
Building: html/pdf, themes (readthedocs)
API docs: .. automodule::, .. autofunction::
Readme.md, contributing, changelog

Demonstrations

Building docs with make html
Auto API reference

Exercise
Document project modules with Sphinx.
Project Integration
Create README and full docs.
Evaluation Criteria

Comprehensive docstrings
Usable built output
Coverage of code


Prompt 35 — Testing (tox, nose, unittest/pyUnit, doctest, pytest)
Teaching Scope
Explain verification strategies, with full suite building.
Concepts to Exhaust

Unit tests: isolation, mocks (unittest.mock)
Integration/end-to-end tests
Frameworks: unittest (TestCase, assert*), pytest (fixtures, parametrize, marks), nose (discovery)
Doctest: tests in docstrings (doctest.testmod)
tox: multi-env testing (tox.ini, envlist)
Coverage (pytest-cov, coverage.py)
TDD/BDD concepts, hypothesis for property-based

Demonstrations

Writing tests with pytest fixtures
Running tox for multi-Python

Exercise
Test project components with unit/integration.
Project Integration
Add /tests directory with coverage.
Evaluation Criteria

High coverage (>80%)
Passing tests with edge cases
Fixture reuse


COMPLETION
After final pass, perform holistic review, assess readiness, and recommend advanced agents via:
https://github.com/Nooran3994/Learn-develop-and-Earn-.git_github-Agents-.git