Python Prompts Guardrail — Mastery Curriculum
Purpose: This document is a comprehensive curriculum execution ledger used by Python_Learning_Guardrail_Co-Pilot.Key Features:
Each prompt fully exhausts its topic(s) conceptually, practically, and diagnostically.
Teaching depth is equivalent to a bootcamp + university-level introduction.
Executed strictly in order and gated by Proceed.


EXECUTION RULES (NON-NEGOTIABLE)

The agent may ONLY teach the currently active prompt.
Every concept must be explained from first principles.
Each prompt MUST include:
Conceptual theory
Mental models
Python syntax and semantics
Common mistakes
Debugging strategies
Real-world analogies

Every prompt modifies the same evolving project.
Advancement requires explicit learner evaluation via Proceed.


STAGE 1 — BEGINNER: LEARN THE BASICS
Prompt 01 — Basic Syntax and What Programming Is
Teaching Scope
Explain what programming means, how humans instruct machines, basic Python syntax rules, whitespace significance, and how Python executes code (top-to-bottom).
Concepts to Exhaust

Source code vs execution
Interpreter loop
Statements vs expressions
Indentation blocks
Why errors stop execution
Comments as non-executable metadata

Demonstrations

Minimal print() program
Correct vs incorrect indentation
Execution order experiment

Exercise
Write a Python script that prints a welcome message, the project name, and a confirmation showing execution order.
Project Integration
Create main.py as the permanent project entry point.
Evaluation Criteria

Correct execution
Correct ordering
No syntax errors


Prompt 02 — Variables and Data Types
Teaching Scope
Explain variables as references to objects in memory, primitive data types, and mutability.
Concepts to Exhaust

Assignment vs equality
Naming conventions
int, float, str, bool
type() inspection
Runtime type errors

Demonstrations

Variable reassignment
Arithmetic with mixed types

Exercise
Declare variables for application name, version, and author; print them formatted.
Project Integration
Introduce a configuration section in main.py.
Evaluation Criteria

Valid variable usage
Correct data type handling


Prompt 03 — Conditionals
Teaching Scope
Explain decision-making using boolean logic and conditional execution.
Concepts to Exhaust

Truth tables
Comparison operators
if/elif/else flow
Logical operators (and, or, not)

Demonstrations

Nested conditionals
Common logic errors

Exercise
Build conditional responses based on user input.
Project Integration
Add logic to control execution paths in main.py.
Evaluation Criteria

Accurate conditional logic
Handling of edge cases


Prompt 04 — Loops
Teaching Scope
Explain iteration, counters, and repetition models.
Concepts to Exhaust

for vs while
Infinite loops
break / continue / else
Loop invariants

Demonstrations

Iterating over ranges and collections
Debugging loop errors

Exercise
Process a collection repeatedly with loops.
Project Integration
Automate repetitive tasks in the project.
Evaluation Criteria

Correct loop termination
Efficient iteration


Prompt 05 — Type Casting
Teaching Scope
Explain implicit vs explicit type conversion and why types matter.
Concepts to Exhaust

Casting functions (int(), str(), etc.)
Casting failures and errors
Type compatibility

Demonstrations

Converting user input
Mixed-type operations

Exercise
Safely convert numeric input and perform calculations.
Project Integration
Validate and cast configuration values.
Evaluation Criteria

Safe type conversions
Error-free casting


Prompt 06 — Exceptions
Teaching Scope
Explain failure handling and defensive programming.
Concepts to Exhaust

Error types (SyntaxError, ValueError, etc.)
Error propagation
try/except/else/finally
Raising exceptions

Demonstrations

Handling invalid input
Custom exception classes

Exercise
Safely handle invalid inputs with try-except.
Project Integration
Stabilize runtime in main.py.
Evaluation Criteria

Proper exception handling
Graceful error recovery


Prompt 07 — Functions and Builtin Functions
Teaching Scope
Explain abstraction, reuse, and built-in functions.
Concepts to Exhaust

Parameters (positional, keyword, defaults)
Return values
Scope (local vs global)
Built-ins (len(), sum(), etc.)
Function composition

Demonstrations

Refactoring code into functions
Variable scope issues

Exercise
Refactor logic into reusable functions.
Project Integration
Modularize the codebase.
Evaluation Criteria

Correct function definitions
Proper scoping


Prompt 08 — Lists, Tuples, Sets
Teaching Scope
Explain grouped data storage and core collections.
Concepts to Exhaust

Mutability differences
Indexing and slicing
Membership testing
Set operations (union, intersection)

Demonstrations

List modifications
Tuple immutability use cases

Exercise
Manipulate lists, tuples, and sets.
Project Integration
Store structured records.
Evaluation Criteria

Correct collection usage
Understanding mutability


Prompt 09 — Dictionaries
Teaching Scope
Explain key-value models and structured mapping.
Concepts to Exhaust

Hashing concepts
Access patterns (get, items)
Dictionary comprehensions
Nested dictionaries

Demonstrations

Building and querying dictionaries
Handling missing keys

Exercise
Create and query dictionaries for data.
Project Integration
Use dictionaries for configuration mapping.
Evaluation Criteria

Efficient key-value operations
Error handling for keys


STAGE 2 — INTERMEDIATE: DATA STRUCTURES & ALGORITHMS
Prompt 10 — Data Structures & Algorithms: Arrays and Linked Lists
Teaching Scope
Explain linear data structures and their implementations.
Concepts to Exhaust

Arrays (lists in Python)
Linked lists (custom implementation)
Time complexities (access, insert, delete)

Demonstrations

Implementing a simple linked list class
Comparing list vs linked list performance

Exercise
Build a linked list and perform operations.
Project Integration
Incorporate a linked list for dynamic data.
Evaluation Criteria

Correct implementation
Understanding trade-offs


Prompt 11 — Heaps, Stacks, and Queues
Teaching Scope
Explain priority and ordered structures.
Concepts to Exhaust

Stack (LIFO), Queue (FIFO)
Heap (heapq module)
Use cases (undo, BFS)

Demonstrations

Using collections.deque for queues
Heap operations

Exercise
Implement stack and queue functionalities.
Project Integration
Add undo/redo using stacks.
Evaluation Criteria

Proper order enforcement
Efficient operations


Prompt 12 — Hash Tables
Teaching Scope
Explain hashing for fast lookups.
Concepts to Exhaust

Hash functions
Collisions and resolution
Dictionaries as hash tables

Demonstrations

Custom hash table simulation
Performance benefits

Exercise
Simulate a hash table.
Project Integration
Optimize lookups in project data.
Evaluation Criteria

Handling collisions
Fast access demonstration


Prompt 13 — Binary Search Tree
Teaching Scope
Explain tree structures for sorted data.
Concepts to Exhaust

Nodes, traversal (in-order, pre-order)
Insertion, deletion, search
Balanced vs unbalanced

Demonstrations

Implementing a BST class
Traversal methods

Exercise
Build and traverse a BST.
Project Integration
Use BST for sorted storage.
Evaluation Criteria

Correct tree operations
Balanced understanding


Prompt 14 — Recursion
Teaching Scope
Explain recursive thinking and base cases.
Concepts to Exhaust

Stack frames
Recursion depth limits
Tail recursion

Demonstrations

Factorial, Fibonacci
Tree traversal recursively

Exercise
Solve problems recursively.
Project Integration
Add recursive data processing.
Evaluation Criteria

Proper base cases
Avoiding stack overflow


Prompt 15 — Sorting Algorithms
Teaching Scope
Explain sorting techniques and efficiencies.
Concepts to Exhaust

Bubble, insertion, merge, quicksort
Time/space complexities
Stable vs unstable

Demonstrations

Implementing merge sort
Comparing efficiencies

Exercise
Implement and test sorting algorithms.
Project Integration
Sort project data collections.
Evaluation Criteria

Correct sorting
Complexity awareness


STAGE 3 — ADVANCED: MODULES, PARADIGMS, AND TOOLS
Prompt 16 — Modules (Builtin and Custom)
Teaching Scope
Explain modularity for scale and organization.
Concepts to Exhaust

Builtin modules (math, random)
Custom modules and imports
__init__.py for packages
Absolute vs relative imports

Demonstrations

Splitting code into modules
Import resolution

Exercise
Refactor project into modules.
Project Integration
Introduce /core and /utils modules.
Evaluation Criteria

Clean imports
No circular dependencies


Prompt 17 — Lambdas
Teaching Scope
Explain anonymous functions for concise code.
Concepts to Exhaust

Lambda syntax
Use in sorting, map/filter
Limitations (no statements)

Demonstrations

Lambda in sorted()
Closures with lambdas

Exercise
Use lambdas in functional operations.
Project Integration
Simplify callbacks in project.
Evaluation Criteria

Appropriate lambda usage
Readability


Prompt 18 — Decorators
Teaching Scope
Explain function wrappers for behavior modification.
Concepts to Exhaust

@decorator syntax
Writing decorators
With arguments

Demonstrations

Timing decorator
Memoization

Exercise
Create and apply decorators.
Project Integration
Add logging/timing to functions.
Evaluation Criteria

Correct wrapping
Preserved metadata


Prompt 19 — Iterators
Teaching Scope
Explain iterable protocols and custom iteration.
Concepts to Exhaust

__iter__ and __next__
StopIteration
Itertools module

Demonstrations

Custom iterator class
Infinite iterators

Exercise
Implement a custom iterator.
Project Integration
Custom data iteration in project.
Evaluation Criteria

Proper protocol implementation
Memory efficiency


Prompt 20 — Regular Expressions
Teaching Scope
Explain pattern matching for text processing.
Concepts to Exhaust

re module (match, search, findall)
Patterns (quantifiers, groups)
Compilation for efficiency

Demonstrations

Email validation
Substitution

Exercise
Validate and extract with regex.
Project Integration
Add input validation layer.
Evaluation Criteria

Accurate patterns
Handling escapes


Prompt 21 — Object-Oriented Programming: Classes and Inheritance
Teaching Scope
Explain OOP principles and class design.
Concepts to Exhaust

Classes as blueprints
Inheritance (single, multiple)
super()
Polymorphism

Demonstrations

Class hierarchies
Method overriding

Exercise
Design classes with inheritance.
Project Integration
Introduce primary project classes.
Evaluation Criteria

Proper encapsulation
Reuse via inheritance


Prompt 22 — Methods and Dunder Methods
Teaching Scope
Explain special methods for customization.
Concepts to Exhaust

Instance, class, static methods
Dunder (init, str, eq)
Operator overloading

Demonstrations

Custom string representation
Comparable objects

Exercise
Implement dunder methods.
Project Integration
Enhance project classes.
Evaluation Criteria

Correct method types
Operator support


Prompt 23 — Package Managers (PyPI, Pip, Conda, Poetry, uv)
Teaching Scope
Explain dependency management tools.
Concepts to Exhaust

PyPI repository
Pip installation
Conda for environments
Poetry for declarative deps
uv for speed

Demonstrations

Installing packages
requirements.txt vs pyproject.toml

Exercise
Set up dependencies for project.
Project Integration
Add external packages.
Evaluation Criteria

Reproducible setup
Conflict resolution


Prompt 24 — Common Packages
Teaching Scope
Introduce essential third-party packages.
Concepts to Exhaust

Requests for HTTP
NumPy/Pandas for data
Selection based on needs

Demonstrations

Fetching data with requests
Basic data manipulation

Exercise
Integrate a common package.
Project Integration
Enhance project with libs.
Evaluation Criteria

Proper integration
Usage understanding


Prompt 25 — Configuration (pyproject.toml)
Teaching Scope
Explain project configuration standards.
Concepts to Exhaust

TOML format
Sections (build-system, tool)
Vs setup.py

Demonstrations

Configuring tools
Reading config in code

Exercise
Create pyproject.toml for project.
Project Integration
Standardize config.
Evaluation Criteria

Valid TOML
Tool integration


Prompt 26 — List Comprehensions and Generator Expressions
Teaching Scope
Explain concise data transformations.
Concepts to Exhaust

Syntax for lists, sets, dicts
Generators for laziness
Nested comprehensions

Demonstrations

Filtering/mapping
Memory usage comparison

Exercise
Refactor loops to comprehensions.
Project Integration
Simplify data processing.
Evaluation Criteria

Readability
Efficiency


Prompt 27 — Paradigms: Context Manager
Teaching Scope
Explain resource management paradigms.
Concepts to Exhaust

with statement
__enter__ and __exit__
contextlib

Demonstrations

File handling with context
Custom managers

Exercise
Implement a context manager.
Project Integration
Manage resources safely.
Evaluation Criteria

Proper cleanup
Exception handling


Prompt 28 — Learn a Framework
Teaching Scope
Explain web frameworks and choices.
Concepts to Exhaust

Synchronous: Pyramid, Plotly Dash
Asynchronous: gevent, aiohttp, Tornado, Sanic
Sync+Async: FastAPI, Django, Flask
Routing, templates, APIs

Demonstrations

Basic app in Flask/FastAPI
Handling requests

Exercise
Build a simple web app.
Project Integration
Add web interface.
Evaluation Criteria

Functional app
Framework understanding


Prompt 29 — Concurrency: Multiprocessing, Asynchrony, GIL, Threading
Teaching Scope
Explain parallel execution models.
Concepts to Exhaust

GIL limitations
Threading for I/O
Multiprocessing for CPU
Asyncio for coroutines

Demonstrations

Threaded vs process pools
Async functions

Exercise
Parallelize tasks.
Project Integration
Optimize performance.
Evaluation Criteria

Correct model choice
Race condition avoidance


Prompt 30 — Environments (Pipenv, virtualenv, pyenv)
Teaching Scope
Explain isolation and version management.
Concepts to Exhaust

Virtualenv creation
Pipenv for deps+env
pyenv for Python versions

Demonstrations

Activating environments
Managing multiple versions

Exercise
Set up project environment.
Project Integration
Ensure reproducibility.
Evaluation Criteria

Isolated setup
Version control


Prompt 31 — Static Typing (typing, mypy, pyright, pyre, Pydantic)
Teaching Scope
Explain type safety and annotations.
Concepts to Exhaust

Type hints
Checkers (mypy, pyright)
Pydantic for validation

Demonstrations

Annotating functions
Running type checks

Exercise
Add types to project.
Project Integration
Improve maintainability.
Evaluation Criteria

Type correctness
Validation usage


Prompt 32 — Code Formatting (yapf, black, ruff)
Teaching Scope
Explain style enforcement.
Concepts to Exhaust

Formatters (black auto-format)
Linters (ruff for errors)
Config options

Demonstrations

Formatting code
Fixing lint issues

Exercise
Format and lint project.
Project Integration
Standardize code quality.
Evaluation Criteria

Consistent style
No lint errors


Prompt 33 — Documentation (Sphinx)
Teaching Scope
Explain professional docs.
Concepts to Exhaust

Docstrings (reST)
Sphinx setup
Auto-generation

Demonstrations

Building docs
API reference

Exercise
Document project.
Project Integration
Create README and docs.
Evaluation Criteria

Comprehensive docs
Usable output


Prompt 34 — Testing (tox, nose, unittest/pyUnit, doctest, pytest)
Teaching Scope
Explain verification strategies.
Concepts to Exhaust

Unit tests
Integration tests
tox for envs
pytest fixtures

Demonstrations

Writing tests
Running suites

Exercise
Test project components.
Project Integration
Add /tests directory.
Evaluation Criteria

High coverage
Passing tests


COMPLETION
After final pass, perform holistic review, assess readiness, and recommend advanced agents via:
https://github.com/Nooran3994/Learn-develop-and-Earn-.git_github-Agents-.git