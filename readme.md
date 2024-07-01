
Python (programming language)

Python

Paradigm	Multi-paradigm: object-oriented,[1] procedural (imperative), functional, structured, reflective
Designed by	Guido van Rossum
Developer	Python Software Foundation
First appeared	20 February 1991; 33 years ago[2]
Stable release	
3.12.4 Edit this on Wikidata / 6 June 2024; 21 days ago
Typing discipline	duck, dynamic, strong;[3] optional type annotations (since 3.5, but those hints are ignored, except with unofficial tools)[4]
OS	Tier 1: 64-bit Linux, macOS; 64- and 32-bit Windows 10+[5]
Tier 2: E.g. 32-bit WebAssembly (WASI) Tier 3: 64-bit FreeBSD, iOS; e.g. Raspberry Pi OS
Unofficial (or has been known to work): Other Unix-like/BSD variants and e.g. Android 5.0+ (official from Python 3.13 planned[6]) and a few other platforms[7][8][9]
License	Python Software Foundation License
Filename extensions	.py, .pyw, .pyz,[10]
.pyi, .pyc, .pyd
Website	python.org
Major implementations
CPython, PyPy, Stackless Python, MicroPython, CircuitPython, IronPython, Jython
Dialects
Cython, RPython, Starlark[11]
Influenced by
ABC,[12] Ada,[13] ALGOL 68,[14]
APL,[15] C,[16] C++,[17] CLU,[18] Dylan,[19]
Haskell,[20][15] Icon,[21] Lisp,[22]
Modula-3,[14][17] Perl,[23] Standard ML[15]
Influenced
Apache Groovy, Boo, Cobra, CoffeeScript,[24] D, F#, GDScript, Genie,[25] Go, JavaScript,[26][27] Julia,[28] Mojo,[29] Nim, Ring,[30] Ruby,[31] Swift[32]
 Python Programming at Wikibooks
Python is a high-level, general-purpose programming language. Its design philosophy emphasizes code readability with the use of significant indentation.[33]

Python is dynamically typed and garbage-collected. It supports multiple programming paradigms, including structured (particularly procedural), object-oriented and functional programming. It is often described as a "batteries included" language due to its comprehensive standard library.[34][35]

Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language and first released it in 1991 as Python 0.9.0.[36] Python 2.0 was released in 2000. Python 3.0, released in 2008, was a major revision not completely backward-compatible with earlier versions. Python 2.7.18, released in 2020, was the last release of Python 2.[37]

Python consistently ranks as one of the most popular programming languages, and has gained widespread use in the machine learning community.[38][39][40][41]

History

The designer of Python, Guido van Rossum, at OSCON 2006
Main article: History of Python
Python was invented in the late 1980s[42] by Guido van Rossum at Centrum Wiskunde & Informatica (CWI) in the Netherlands as a successor to the ABC programming language, which was inspired by SETL,[43] capable of exception handling and interfacing with the Amoeba operating system.[12] Its implementation began in December 1989.[44] Van Rossum shouldered sole responsibility for the project, as the lead developer, until 12 July 2018, when he announced his "permanent vacation" from his responsibilities as Python's "benevolent dictator for life" (BDFL), a title the Python community bestowed upon him to reflect his long-term commitment as the project's chief decision-maker[45] (he's since come out of retirement and is self-titled "BDFL-emeritus"). In January 2019, active Python core developers elected a five-member Steering Council to lead the project.[46][47]

Python 2.0 was released on 16 October 2000, with many major new features such as list comprehensions, cycle-detecting garbage collection, reference counting, and Unicode support.[48] Python 3.0, released on 3 December 2008, with many of its major features backported to Python 2.6.x[49] and 2.7.x. Releases of Python 3 include the 2to3 utility, which automates the translation of Python 2 code to Python 3.[50]

Python 2.7's end-of-life was initially set for 2015, then postponed to 2020 out of concern that a large body of existing code could not easily be forward-ported to Python 3.[51][52] No further security patches or other improvements will be released for it.[53][54] Currently only 3.8 and later are supported (2023 security issues were fixed in e.g. 3.7.17, the final 3.7.x release[55]). While Python 2.7 and older is officially unsupported, a different unofficial Python implementation, PyPy, continues to support Python 2, i.e. "2.7.18+" (plus 3.9 and 3.10), with the plus meaning (at least some) "backported security updates".[56]

In 2021 (and again twice in 2022), security updates were expedited, since all Python versions were insecure (including 2.7[57]) because of security issues leading to possible remote code execution[58] and web-cache poisoning.[59] In 2022, Python 3.10.4 and 3.9.12 were expedited[60] and 3.8.13, because of many security issues.[61] When Python 3.9.13 was released in May 2022, it was announced that the 3.9 series (joining the older series 3.8 and 3.7) would only receive security fixes in the future.[62] On 7 September 2022, four new releases were made due to a potential denial-of-service attack: 3.10.7, 3.9.14, 3.8.14, and 3.7.14.[63][64]

As of October 2023, Python 3.12 is the stable release, and 3.12 and 3.11 are the only versions with active (as opposed to just security) support. Notable changes in 3.11 from 3.10 include increased program execution speed and improved error reporting.[65]

Every Python release since 3.5 has added some syntax to the language. 3.10 added the | union type operator [66] and the match and case keywords (for structural pattern matching statements). 3.11 expanded exception handling functionality. Python 3.12 added the new keyword type.

Python 3.11 claims to be between 10 and 60% faster than Python 3.10, and Python 3.12 adds another 5% on top of that. It also has improved error messages, and many other changes.

Since 27 June 2023, Python 3.8 is the oldest supported version of Python (albeit in the 'security support' phase), due to Python 3.7 reaching end-of-life.[67]

Python 3.13 introduced an incremental garbage collector (producing shorter pauses for collection in programs with a lot of objects); an experimental JIT compiler;[68] and removals from the C API. Some standard library modules and many deprecated classes, functions and methods, will be removed in Python 3.15 and or 3.16.[69][70] Starting with 3.13, it and later versions have 2 years of full support (up from one and a half); followed by 3 years of security support (for same total support as before).

Design philosophy and features
Python is a multi-paradigm programming language. Object-oriented programming and structured programming are fully supported, and many of their features support functional programming and aspect-oriented programming (including metaprogramming[71] and metaobjects).[72] Many other paradigms are supported via extensions, including design by contract[73][74] and logic programming.[75]

Python uses dynamic typing and a combination of reference counting and a cycle-detecting garbage collector for memory management.[76] It uses dynamic name resolution (late binding), which binds method and variable names during program execution.

Its design offers some support for functional programming in the Lisp tradition. It has filter,mapandreduce functions; list comprehensions, dictionaries, sets, and generator expressions.[77] The standard library has two modules (itertools and functools) that implement functional tools borrowed from Haskell and Standard ML.[78]

Its core philosophy is summarized in the Zen of Python (PEP 20), which includes aphorisms such as:[79]

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Readability counts.
However, Python features regularly violate these principles and received criticism for adding unnecessary language bloat.[80][81] Responses to these criticisms are that the Zen of Python is a guideline rather than a rule.[82] The addition of some new features had been so controversial that Guido van Rossum resigned as Benevolent Dictator for Life following vitriol over the addition of the assignment expression operator in Python 3.8.[83][84]

Nevertheless, rather than building all of its functionality into its core, Python was designed to be highly extensible via modules. This compact modularity has made it particularly popular as a means of adding programmable interfaces to existing applications. Van Rossum's vision of a small core language with a large standard library and easily extensible interpreter stemmed from his frustrations with ABC, which espoused the opposite approach.[42]

Python claims to strive for a simpler, less-cluttered syntax and grammar while giving developers a choice in their coding methodology. In contrast to Perl's "there is more than one way to do it" motto, Python embraces a "there should be one—and preferably only one—obvious way to do it." philosophy.[79] In practice, however, Python provides many ways to achieve the same task. There are, for example, at least three ways to format a string literal, with no certainty as to which one a programmer should use.[85] Alex Martelli, a Fellow at the Python Software Foundation and Python book author, wrote: "To describe something as 'clever' is not considered a compliment in the Python culture."[86]

Python's developers usually strive to avoid premature optimization and reject patches to non-critical parts of the CPython reference implementation that would offer marginal increases in speed at the cost of clarity.[87] Execution speed can be improved by moving speed-critical functions to extension modules written in languages such as C, or by using a just-in-time compiler like PyPy. It is also possible to cross-compile to other languages, but it either doesn't provide the full speed-up that might be expected, since Python is a very dynamic language, or a restricted subset of Python is compiled, and possibly semantics are slightly changed.[88]

Python's developers aim for it to be fun to use. This is reflected in its name—a tribute to the British comedy group Monty Python[89]—and in occasionally playful approaches to tutorials and reference materials, such as the use of the terms "spam" and "eggs" (a reference to a Monty Python sketch) in examples, instead of the often-used "foo" and "bar".[90][91] A common neologism in the Python community is pythonic, which has a wide range of meanings related to program style. "Pythonic" code may use Python idioms well, be natural or show fluency in the language, or conform with Python's minimalist philosophy and emphasis on readability. Code that is difficult to understand or reads like a rough transcription from another programming language is called unpythonic.[92]

Syntax and semantics
Main article: Python syntax and semantics
Python is meant to be an easily readable language. Its formatting is visually uncluttered and often uses English keywords where other languages use punctuation. Unlike many other languages, it does not use curly brackets to delimit blocks, and semicolons after statements are allowed but rarely used. It has fewer syntactic exceptions and special cases than C or Pascal.[93]

Indentation
Main article: Python syntax and semantics § Indentation
Python uses whitespace indentation, rather than curly brackets or keywords, to delimit blocks. An increase in indentation comes after certain statements; a decrease in indentation signifies the end of the current block.[94] Thus, the program's visual structure accurately represents its semantic structure.[95] This feature is sometimes termed the off-side rule. Some other languages use indentation this way; but in most, indentation has no semantic meaning. The recommended indent size is four spaces.[96]

Statements and control flow
Python's statements include:

The assignment statement, using a single equals sign =
The if statement, which conditionally executes a block of code, along with else and elif (a contraction of else-if)
The for statement, which iterates over an iterable object, capturing each element to a local variable for use by the attached block
The while statement, which executes a block of code as long as its condition is true
The try statement, which allows exceptions raised in its attached code block to be caught and handled by except clauses (or new syntax except* in Python 3.11 for exception groups[97]); it also ensures that clean-up code in a finally block is always run regardless of how the block exits
The raise statement, used to raise a specified exception or re-raise a caught exception
The class statement, which executes a block of code and attaches its local namespace to a class, for use in object-oriented programming
The def statement, which defines a function or method
The with statement, which encloses a code block within a context manager (for example, acquiring a lock before it is run, then releasing the lock; or opening and closing a file), allowing resource-acquisition-is-initialization (RAII)-like behavior and replacing a common try/finally idiom[98]
The break statement, which exits a loop
The continue statement, which skips the rest of the current iteration and continues with the next
The del statement, which removes a variable—deleting the reference from the name to the value, and producing an error if the variable is referred to before it is redefined
The pass statement, serving as a NOP, syntactically needed to create an empty code block
The assert statement, used in debugging to check for conditions that should apply
The yield statement, which returns a value from a generator function (and also an operator); used to implement coroutines
The return statement, used to return a value from a function
The import and from statements, used to import modules whose functions or variables can be used in the current program
The assignment statement (=) binds a name as a reference to a separate, dynamically allocated object. Variables may subsequently be rebound at any time to any object. In Python, a variable name is a generic reference holder without a fixed data type; however, it always refers to some object with a type. This is called dynamic typing—in contrast to statically-typed languages, where each variable may contain only a value of a certain type.

Python does not support tail call optimization or first-class continuations, and, according to Van Rossum, it never will.[99][100] However, better support for coroutine-like functionality is provided by extending Python's generators.[101] Before 2.5, generators were lazy iterators; data was passed unidirectionally out of the generator. From Python 2.5 on, it is possible to pass data back into a generator function; and from version 3.3, it can be passed through multiple stack levels.[102]

Expressions
Python's expressions include:

The +, -, and * operators for mathematical addition, subtraction, and multiplication are similar to other languages, but the behavior of division differs. There are two types of divisions in Python: floor division (or integer division) // and floating-point/division.[103] Python uses the ** operator for exponentiation.
Python uses the + operator for string concatenation. Python uses the * operator for duplicating a string a specified number of times.
The @ infix operator. It is intended to be used by libraries such as NumPy for matrix multiplication.[104][105]
The syntax :=, called the "walrus operator", was introduced in Python 3.8. It assigns values to variables as part of a larger expression.[106]
In Python, == compares by value. Python's is operator may be used to compare object identities (comparison by reference), and comparisons may be chained—for example, a <= b <= c.
Python uses and, or, and not as Boolean operators.
Python has a type of expression named a list comprehension, and a more general expression named a generator expression.[77]
Anonymous functions are implemented using lambda expressions; however, there may be only one expression in each body.
Conditional expressions are written as x if c else y[107] (different in order of operands from the c ? x : y operator common to many other languages).
Python makes a distinction between lists and tuples. Lists are written as [1, 2, 3], are mutable, and cannot be used as the keys of dictionaries (dictionary keys must be immutable in Python). Tuples, written as (1, 2, 3), are immutable and thus can be used as keys of dictionaries, provided all of the tuple's elements are immutable. The + operator can be used to concatenate two tuples, which does not directly modify their contents, but produces a new tuple containing the elements of both. Thus, given the variable t initially equal to (1, 2, 3), executing t = t + (4, 5) first evaluates t + (4, 5), which yields (1, 2, 3, 4, 5), which is then assigned back to t—thereby effectively "modifying the contents" of t while conforming to the immutable nature of tuple objects. Parentheses are optional for tuples in unambiguous contexts.[108]
Python features sequence unpacking where multiple expressions, each evaluating to anything that can be assigned (to a variable, writable property, etc.) are associated in an identical manner to that forming tuple literals—and, as a whole, are put on the left-hand side of the equal sign in an assignment statement. The statement expects an iterable object on the right-hand side of the equal sign that produces the same number of values as the provided writable expressions; when iterated through them, it assigns each of the produced values to the corresponding expression on the left.[109]
Python has a "string format" operator % that functions analogously to printf format strings in C—e.g. "spam=%s eggs=%d" % ("blah", 2) evaluates to "spam=blah eggs=2". In Python 2.6+ and 3+, this was supplemented by the format() method of the str class, e.g. "spam={0} eggs={1}".format("blah", 2). Python 3.6 added "f-strings": spam = "blah"; eggs = 2; f'spam={spam} eggs={eggs}'.[110]
Strings in Python can be concatenated by "adding" them (with the same operator as for adding integers and floats), e.g. "spam" + "eggs" returns "spameggs". If strings contain numbers, they are added as strings rather than integers, e.g. "2" + "2" returns "22".
Python has various string literals:
Delimited by single or double quotes; unlike in Unix shells, Perl, and Perl-influenced languages, single and double quotes work the same. Both use the backslash (\) as an escape character. String interpolation became available in Python 3.6 as "formatted string literals".[110]
Triple-quoted (beginning and ending with three single or double quotes), which may span multiple lines and function like here documents in shells, Perl, and Ruby.
Raw string varieties, denoted by prefixing the string literal with r. Escape sequences are not interpreted; hence raw strings are useful where literal backslashes are common, such as regular expressions and Windows-style paths. (Compare "@-quoting" in C#.)
Python has array index and array slicing expressions in lists, denoted as a[key], a[start:stop] or a[start:stop:step]. Indexes are zero-based, and negative indexes are relative to the end. Slices take elements from the start index up to, but not including, the stop index. The third slice parameter, called step or stride, allows elements to be skipped and reversed. Slice indexes may be omitted—for example, a[:] returns a copy of the entire list. Each element of a slice is a shallow copy.
In Python, a distinction between expressions and statements is rigidly enforced, in contrast to languages such as Common Lisp, Scheme, or Ruby. This leads to duplicating some functionality. For example:

List comprehensions vs. for-loops
Conditional expressions vs. if blocks
The eval() vs. exec() built-in functions (in Python 2, exec is a statement); the former is for expressions, the latter is for statements
Statements cannot be a part of an expression—so list and other comprehensions or lambda expressions, all being expressions, cannot contain statements. A particular case is that an assignment statement such as a = 1 cannot form part of the conditional expression of a conditional statement.

Methods
Methods on objects are functions attached to the object's class; the syntax instance.method(argument) is, for normal methods and functions, syntactic sugar for Class.method(instance, argument). Python methods have an explicit self parameter to access instance data, in contrast to the implicit self (or this) in some other object-oriented programming languages (e.g., C++, Java, Objective-C, Ruby).[111] Python also provides methods, often called dunder methods (due to their names beginning and ending with double-underscores), to allow user-defined classes to modify how they are handled by native operations including length, comparison, in arithmetic operations and type conversion.[112]

Typing

The standard type hierarchy in Python 3
Python uses duck typing and has typed objects but untyped variable names. Type constraints are not checked at compile time; rather, operations on an object may fail, signifying that it is not of a suitable type. Despite being dynamically typed, Python is strongly typed, forbidding operations that are not well-defined (for example, adding a number to a string) rather than silently attempting to make sense of them.

Python allows programmers to define their own types using classes, most often used for object-oriented programming. New instances of classes are constructed by calling the class (for example, SpamClass() or EggsClass()), and the classes are instances of the metaclass type (itself an instance of itself), allowing metaprogramming and reflection.

Before version 3.0, Python had two kinds of classes (both using the same syntax): old-style and new-style;[113] current Python versions only support the semantics of the new style.

Python supports optional type annotations.[4][114] These annotations are not enforced by the language, but may be used by external tools such as mypy to catch errors.[115][116] Mypy also supports a Python compiler called mypyc, which leverages type annotations for optimization.[117]

Summary of Python 3's built-in types
Type	Mutability	Description	Syntax examples
bool	immutable	Boolean value	True
False
bytearray	mutable	Sequence of bytes	bytearray(b'Some ASCII')
bytearray(b"Some ASCII")
bytearray([119, 105, 107, 105])
bytes	immutable	Sequence of bytes	b'Some ASCII'
b"Some ASCII"
bytes([119, 105, 107, 105])
complex	immutable	Complex number with real and imaginary parts	3+2.7j
3 + 2.7j
dict	mutable	Associative array (or dictionary) of key and value pairs; can contain mixed types (keys and values), keys must be a hashable type	{'key1': 1.0, 3: False}
{}
types.EllipsisType	immutable	An ellipsis placeholder to be used as an index in NumPy arrays	...
Ellipsis
float	immutable	Double-precision floating-point number. The precision is machine-dependent but in practice is generally implemented as a 64-bit IEEE 754 number with 53 bits of precision.[118]	
1.33333

frozenset	immutable	Unordered set, contains no duplicates; can contain mixed types, if hashable	frozenset([4.0, 'string', True])
int	immutable	Integer of unlimited magnitude[119]	42
list	mutable	List, can contain mixed types	[4.0, 'string', True]
[]
types.NoneType	immutable	An object representing the absence of a value, often called null in other languages	None
types.NotImplementedType	immutable	A placeholder that can be returned from overloaded operators to indicate unsupported operand types.	NotImplemented
range	immutable	An immutable sequence of numbers commonly used for looping a specific number of times in for loops[120]	range(-1, 10)
range(10, -5, -2)
set	mutable	Unordered set, contains no duplicates; can contain mixed types, if hashable	{4.0, 'string', True}
set()
str	immutable	A character string: sequence of Unicode codepoints	'Wikipedia'
"Wikipedia"
"""Spanning
multiple
lines"""
Spanning
multiple
lines
tuple	immutable	Can contain mixed types	(4.0, 'string', True)
('single element',)
()
Arithmetic operations
Python has the usual symbols for arithmetic operators (+, -, *, /), the floor division operator // and the modulo operation % (where the remainder can be negative, e.g. 4 % -3 == -2). It also has ** for exponentiation, e.g. 5**3 == 125 and 9**0.5 == 3.0, and a matrix‑multiplication operator @ .[121] These operators work like in traditional math; with the same precedence rules, the operators infix (+ and - can also be unary to represent positive and negative numbers respectively).

The division between integers produces floating-point results. The behavior of division has changed significantly over time:[122]

Current Python (i.e. since 3.0) changed / to always be floating-point division, e.g. 5/2 == 2.5.
The floor division // operator was introduced. So 7//3 == 2, -7//3 == -3, 7.5//3 == 2.0 and -7.5//3 == -3.0. Adding from __future__ import division causes a module used in Python 2.7 to use Python 3.0 rules for division (see above).
In Python terms, / is true division (or simply division), and // is floor division. / before version 3.0 is classic division.[122]

Rounding towards negative infinity, though different from most languages, adds consistency. For instance, it means that the equation (a + b)//b == a//b + 1 is always true. It also means that the equation b*(a//b) + a%b == a is valid for both positive and negative values of a. However, maintaining the validity of this equation means that while the result of a%b is, as expected, in the half-open interval [0, b), where b is a positive integer, it has to lie in the interval (b, 0] when b is negative.[123]

Python provides a round function for rounding a float to the nearest integer. For tie-breaking, Python 3 uses round to even: round(1.5) and round(2.5) both produce 2.[124] Versions before 3 used round-away-from-zero: round(0.5) is 1.0, round(-0.5) is −1.0.[125]

Python allows Boolean expressions with multiple equality relations in a manner that is consistent with general use in mathematics. For example, the expression a < b < c tests whether a is less than b and b is less than c.[126] C-derived languages interpret this expression differently: in C, the expression would first evaluate a < b, resulting in 0 or 1, and that result would then be compared with c.[127]

Python uses arbitrary-precision arithmetic for all integer operations. The Decimal type/class in the decimal module provides decimal floating-point numbers to a pre-defined arbitrary precision and several rounding modes.[128] The Fraction class in the fractions module provides arbitrary precision for rational numbers.[129]

Due to Python's extensive mathematics library, and the third-party library NumPy that further extends the native capabilities, it is frequently used as a scientific scripting language to aid in problems such as numerical data processing and manipulation.[130][131]

Programming examples
"Hello, World!" program:

print('Hello, world!')
Program to calculate the factorial of a positive integer:

n = int(input('Type a number, and its factorial will be printed: '))

if n < 0:
    raise ValueError('You must enter a non-negative integer')

factorial = 1
for i in range(2, n + 1):
    factorial *= i

print(factorial)
Libraries
Python's large standard library[132] provides tools suited to many tasks and is commonly cited as one of its greatest strengths. For Internet-facing applications, many standard formats and protocols such as MIME and HTTP are supported. It includes modules for creating graphical user interfaces, connecting to relational databases, generating pseudorandom numbers, arithmetic with arbitrary-precision decimals,[128] manipulating regular expressions, and unit testing.

Some parts of the standard library are covered by specifications—for example, the Web Server Gateway Interface (WSGI) implementation wsgiref follows PEP 333[133]—but most are specified by their code, internal documentation, and test suites. However, because most of the standard library is cross-platform Python code, only a few modules need altering or rewriting for variant implementations.

As of 17 March 2024, the Python Package Index (PyPI), the official repository for third-party Python software, contains over 523,000[134] packages with a wide range of functionality, including:

Automation
Data analytics
Databases
Documentation
Graphical user interfaces
Image processing
Machine learning
Mobile apps
Multimedia
Computer networking
Scientific computing
System administration
Test frameworks
Text processing
Web frameworks
Web scraping
Development environments
See also: Comparison of integrated development environments § Python
Most Python implementations (including CPython) include a read–eval–print loop (REPL), permitting them to function as a command line interpreter for which users enter statements sequentially and receive results immediately.

Python also comes with an Integrated development environment (IDE) called IDLE, which is more beginner-oriented.

Other shells, including IDLE and IPython, add further abilities such as improved auto-completion, session state retention, and syntax highlighting.

As well as standard desktop integrated development environments including PyCharm, IntelliJ Idea, Visual Studio Code etc, there are web browser-based IDEs, including SageMath, for developing science- and math-related programs; PythonAnywhere, a browser-based IDE and hosting environment; and Canopy IDE, a commercial IDE emphasizing scientific computing.[135]

Implementations
See also: List of Python software § Python implementations
Reference implementation
CPython is the reference implementation of Python. It is written in C, meeting the C89 standard (Python 3.11 uses C11[136]) with several select C99 features. CPython includes its own C extensions, but third-party extensions are not limited to older C versions—e.g. they can be implemented with C11 or C++.[137][138] CPython compiles Python programs into an intermediate bytecode[139] which is then executed by its virtual machine.[140] CPython is distributed with a large standard library written in a mixture of C and native Python, and is available for many platforms, including Windows (starting with Python 3.9, the Python installer deliberately fails to install on Windows 7 and 8;[141][142] Windows XP was supported until Python 3.5) and most modern Unix-like systems, including macOS (and Apple M1 Macs, since Python 3.9.1, with experimental installer), with unofficial support for VMS.[143] Platform portability was one of its earliest priorities.[144] (During Python 1 and 2 development, even OS/2 and Solaris were supported,[145] but support has since been dropped for many platforms.)

Python, since 3.7, only supports operating systems with multi-threading support.

Other implementations
PyPy is a fast, compliant interpreter of Python 2.7 and 3.8.[146][147] Its just-in-time compiler often brings a significant speed improvement over CPython, but some libraries written in C cannot be used with it.[148]
Stackless Python is a significant fork of CPython that implements microthreads; it does not use the call stack in the same way, thus allowing massively concurrent programs. PyPy also has a stackless version.[149]
MicroPython and CircuitPython are Python 3 variants optimized for microcontrollers, including Lego Mindstorms EV3.[150]
Pyston is a variant of the Python runtime that uses just-in-time compilation to speed up the execution of Python programs.[151]
Cinder is a performance-oriented fork of CPython 3.8 that contains a number of optimizations, including bytecode inline caching, eager evaluation of coroutines, a method-at-a-time JIT, and an experimental bytecode compiler.[152]
Snek[153][154][155] Embedded Computing Language (compatible with e.g. 8-bit AVR microcontrollers such as ATmega 328P-based Arduino, as well as larger ones compatible with MicroPython) "is Python-inspired, but it is not Python. It is possible to write Snek programs that run under a full Python system, but most Python programs will not run under Snek."[156] It is an imperative language not including OOP / classes, unlike Python, and simplifying to one number type with 32-bit single-precision (similar to JavaScript, except smaller).
Unsupported implementations
Other just-in-time Python compilers have been developed, but are now unsupported:

Google began a project named Unladen Swallow in 2009, with the aim of speeding up the Python interpreter five-fold by using the LLVM, and of improving its multithreading ability to scale to thousands of cores,[157] while ordinary implementations suffer from the global interpreter lock.
Psyco is a discontinued just-in-time specializing compiler that integrates with CPython and transforms bytecode to machine code at runtime. The emitted code is specialized for certain data types and is faster than the standard Python code. Psyco does not support Python 2.7 or later.
PyS60 was a Python 2 interpreter for Series 60 mobile phones released by Nokia in 2005. It implemented many of the modules from the standard library and some additional modules for integrating with the Symbian operating system. The Nokia N900 also supports Python with GTK widget libraries, enabling programs to be written and run on the target device.[158]
Cross-compilers to other languages
There are several compilers/transpilers to high-level object languages, with either unrestricted Python, a restricted subset of Python, or a language similar to Python as the source language:

Brython,[159] Transcrypt[160][161] and Pyjs (latest release in 2012) compile Python to JavaScript.
Codon compiles a subset of statically typed Python[162] to machine code (via LLVM) and supports native multithreading.[163]
Cython compiles (a superset of) Python to C. The resulting code is also usable with Python via direct C-level API calls into the Python interpreter.
PyJL compiles/transpiles a subset of Python to "human-readable, maintainable, and high-performance Julia source code".[88] Despite claiming high performance, no tool can claim to do that for arbitrary Python code; i.e. it's known not possible to compile to a faster language or machine code. Unless semantics of Python are changed, but in many cases speedup is possible with few or no changes in the Python code. The faster Julia source code can then be used from Python, or compiled to machine code, and based that way.
Nuitka compiles Python into C.[164]
Numba uses LLVM to compile a subset of Python to machine code.
Pythran compiles a subset of Python 3 to C++ (C++11).[165]
RPython can be compiled to C, and is used to build the PyPy interpreter of Python.
The Python → 11l → C++ transpiler[166] compiles a subset of Python 3 to C++ (C++17).
Specialized:

MyHDL is a Python-based hardware description language (HDL), that converts MyHDL code to Verilog or VHDL code.
Older projects (or not to be used with Python 3.x and latest syntax):

Google's Grumpy (latest release in 2017) transpiles Python 2 to Go.[167][168][169]
IronPython allows running Python 2.7 programs (and an alpha, released in 2021, is also available for "Python 3.4, although features and behaviors from later versions may be included"[170]) on the .NET Common Language Runtime.[171]
Jython compiles Python 2.7 to Java bytecode, allowing the use of the Java libraries from a Python program.[172]
Pyrex (latest release in 2010) and Shed Skin (latest release in 2013) compile to C and C++ respectively.
Performance
Performance comparison of various Python implementations on a non-numerical (combinatorial) workload was presented at EuroSciPy '13.[173] Python's performance compared to other programming languages is also benchmarked by The Computer Language Benchmarks Game.[174]

Development
Python's development is conducted largely through the Python Enhancement Proposal (PEP) process, the primary mechanism for proposing major new features, collecting community input on issues, and documenting Python design decisions.[175] Python coding style is covered in PEP 8.[176] Outstanding PEPs are reviewed and commented on by the Python community and the steering council.[175]

Enhancement of the language corresponds with the development of the CPython reference implementation. The mailing list python-dev is the primary forum for the language's development. Specific issues were originally discussed in the Roundup bug tracker hosted at by the foundation.[177] In 2022, all issues and discussions were migrated to GitHub.[178] Development originally took place on a self-hosted source-code repository running Mercurial, until Python moved to GitHub in January 2017.[179]

CPython's public releases come in three types, distinguished by which part of the version number is incremented:

Backward-incompatible versions, where code is expected to break and needs to be manually ported. The first part of the version number is incremented. These releases happen infrequently—version 3.0 was released 8 years after 2.0. According to Guido van Rossum, a version 4.0 is very unlikely to ever happen.[180]
Major or "feature" releases are largely compatible with the previous version but introduce new features. The second part of the version number is incremented. Starting with Python 3.9, these releases are expected to happen annually.[181][182] Each major version is supported by bug fixes for several years after its release.[183]
Bugfix releases,[184] which introduce no new features, occur about every 3 months and are made when a sufficient number of bugs have been fixed upstream since the last release. Security vulnerabilities are also patched in these releases. The third and final part of the version number is incremented.[184]
Many alpha, beta, and release-candidates are also released as previews and for testing before final releases. Although there is a rough schedule for each release, they are often delayed if the code is not ready. Python's development team monitors the state of the code by running the large unit test suite during development.[185]

The major academic conference on Python is PyCon. There are also special Python mentoring programs, such as PyLadies.

Python 3.12 removed wstr meaning Python extensions[186] need to be modified,[187] and 3.10 added pattern matching to the language.[188]

Python 3.12 dropped some outdated modules, and more will be dropped in the future, deprecated as of 3.13; already deprecated array 'u' format code will emit DeprecationWarning since 3.13 and will be removed in Python 3.16. The 'w' format code should be used instead. Part of ctypes is also deprecated and http.server.CGIHTTPRequestHandler will emit a DeprecationWarning, and will be removed in 3.15. Using that code already has a high potential for both security and functionality bugs. Parts of the typing module are deprecated, e.g. creating a typing.NamedTuple class using keyword arguments to denote the fields and such (and more) will be disallowed in Python 3.15.

API documentation generators
Tools that can generate documentation for Python API include pydoc (available as part of the standard library), Sphinx, Pdoc and its forks, Doxygen and Graphviz, among others.[189]

Naming
Python's name is derived from the British comedy group Monty Python, whom Python creator Guido van Rossum enjoyed while developing the language. Monty Python references appear frequently in Python code and culture;[190] for example, the metasyntactic variables often used in Python literature are spam and eggs instead of the traditional foo and bar.[190][191] The official Python documentation also contains various references to Monty Python routines.[192][193] Users of Python are sometimes referred to as "Pythonistas".[194]

The prefix Py- is used to show that something is related to Python. Examples of the use of this prefix in names of Python applications or libraries include Pygame, a binding of SDL to Python (commonly used to create games); PyQt and PyGTK, which bind Qt and GTK to Python respectively; and PyPy, a Python implementation originally written in Python.

Popularity
Since 2003, Python has consistently ranked in the top ten most popular programming languages in the TIOBE Programming Community Index where as of December 2022 it was the most popular language (ahead of C, C++, and Java).[40] It was selected as Programming Language of the Year (for "the highest rise in ratings in a year") in 2007, 2010, 2018, and 2020 (the only language to have done so four times as of 2020[195]).

Large organizations that use Python include Wikipedia, Google,[196] Yahoo!,[197] CERN,[198] NASA,[199] Facebook,[200] Amazon, Instagram,[201] Spotify,[202] and some smaller entities like ILM[203] and ITA.[204] The social news networking site Reddit was written mostly in Python.[205]

Uses
Main article: List of Python software

Python Powered
Python can serve as a scripting language for web applications, e.g. via mod_wsgi for the Apache webserver.[206] With Web Server Gateway Interface, a standard API has evolved to facilitate these applications. Web frameworks like Django, Pylons, Pyramid, TurboGears, web2py, Tornado, Flask, Bottle, and Zope support developers in the design and maintenance of complex applications. Pyjs and IronPython can be used to develop the client-side of Ajax-based applications. SQLAlchemy can be used as a data mapper to a relational database. Twisted is a framework to program communications between computers, and is used (for example) by Dropbox.

Libraries such as NumPy, SciPy and Matplotlib allow the effective use of Python in scientific computing,[207][208] with specialized libraries such as Biopython and Astropy providing domain-specific functionality. SageMath is a computer algebra system with a notebook interface programmable in Python: its library covers many aspects of mathematics, including algebra, combinatorics, numerical mathematics, number theory, and calculus.[209] OpenCV has Python bindings with a rich set of features for computer vision and image processing.[210]

Python is commonly used in artificial intelligence projects and machine learning projects with the help of libraries like TensorFlow, Keras, Pytorch, scikit-learn and the Logic language ProbLog.[211][212][213][214][215] As a scripting language with a modular architecture, simple syntax, and rich text processing tools, Python is often used for natural language processing.[216]

The combination of Python and Prolog has proved to be particularly useful for AI applications, with Prolog providing knowledge representation and reasoning capablities. The Janus system, in particular, exploits the similarites between these two languages, in part because of their use of dynamic typing, and the simple recursive nature of their data structures. Typical applications of this combination include natural language processing, visual query answering, geospatial reasoning, and handling of semantic web data.[217][218] The Natlog system, implemented in Python, uses Definite Clause Grammars (DCGs) as prompt generators for text-to-text generators like GPT3 and text-to-image generators like DALL-E or Stable Diffusion.[219]

Python can also be used for graphical user interface (GUI) by using libraries like Tkinter.[220][221]

Python has been successfully embedded in many software products as a scripting language, including in finite element method software such as Abaqus, 3D parametric modelers like FreeCAD, 3D animation packages such as 3ds Max, Blender, Cinema 4D, Lightwave, Houdini, Maya, modo, MotionBuilder, Softimage, the visual effects compositor Nuke, 2D imaging programs like GIMP,[222] Inkscape, Scribus and Paint Shop Pro,[223] and musical notation programs like scorewriter and capella. GNU Debugger uses Python as a pretty printer to show complex structures such as C++ containers. Esri promotes Python as the best choice for writing scripts in ArcGIS.[224] It has also been used in several video games,[225][226] and has been adopted as first of the three available programming languages in Google App Engine, the other two being Java and Go.[227]

Many operating systems include Python as a standard component. It ships with most Linux distributions,[228] AmigaOS 4 (using Python 2.7), FreeBSD (as a package), NetBSD, and OpenBSD (as a package) and can be used from the command line (terminal). Many Linux distributions use installers written in Python: Ubuntu uses the Ubiquity installer, while Red Hat Linux and Fedora Linux use the Anaconda installer. Gentoo Linux uses Python in its package management system, Portage.

Python is used extensively in the information security industry, including in exploit development.[229][230]

Most of the Sugar software for the One Laptop per Child XO, developed at Sugar Labs as of 2008, is written in Python.[231] The Raspberry Pi single-board computer project has adopted Python as its main user-programming language.

LibreOffice includes Python and intends to replace Java with Python. Its Python Scripting Provider is a core feature[232] since Version 4.0 from 7 February 2013.

Languages influenced by Python
Python's design and philosophy have influenced many other programming languages:

Boo uses indentation, a similar syntax, and a similar object model.[233]
Cobra uses indentation and a similar syntax, and its Acknowledgements document lists Python first among languages that influenced it.[234]
CoffeeScript, a programming language that cross-compiles to JavaScript, has Python-inspired syntax.
ECMAScript–JavaScript borrowed iterators and generators from Python.[235]
GDScript, a scripting language very similar to Python, built-in to the Godot game engine.[236]
Go is designed for the "speed of working in a dynamic language like Python"[237] and shares the same syntax for slicing arrays.
Groovy was motivated by the desire to bring the Python design philosophy to Java.[238]
Julia was designed to be "as usable for general programming as Python".[28]
Mojo is a non-strict[29][239] superset of Python (e.g. still missing classes, and adding e.g. struct).[240]
Nim uses indentation and similar syntax.[241]
Ruby's creator, Yukihiro Matsumoto, has said: "I wanted a scripting language that was more powerful than Perl, and more object-oriented than Python. That's why I decided to design my own language."[242]
Swift, a programming language developed by Apple, has some Python-inspired syntax.[243]
Kotlin blends Python and Java features, minimizing boilerplate code for enhanced developer efficiency.[244]
Python's development practices have also been emulated by other languages. For example, the practice of requiring a document describing the rationale for, and issues surrounding, a change to the language (in Python, a PEP) is also used in Tcl,[245] Erlang,[246] and Swift.[247]
