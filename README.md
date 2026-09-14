# Regex Engine

A regular expression engine written in **C++**, built as a learning project to better understand how regex parsing and pattern matching work internally.

Instead of relying on C++'s built-in `std::regex`, this project explores the lower-level process of representing and interpreting regular expressions.

## Overview

Regular expressions are usually treated as a black box: provide a pattern, provide a string, and receive a match result.

This project was created to explore what happens underneath that abstraction.

The engine focuses on the parsing side of regular expressions and serves as an experiment in concepts commonly found in compilers and interpreters, including:

* Parsing structured expressions
* Representing regex operations internally
* Handling nested expressions
* Working with operators and pattern components
* Designing C++ abstractions for syntax processing

## Project Structure

```text
Regex-Engine/
├── Parser/
│   └── ...
├── premake5.lua
└── .gitignore
```

The main implementation is located inside the `Parser` directory.

The project uses **Premake** to generate build files.

## Building

### Requirements

* C++ compiler
* Premake5
* 64-bit development environment

Clone the repository:

```bash
git clone https://github.com/akmalm07/Regex-Engine.git
cd Regex-Engine
```

Generate project files with Premake.

For Visual Studio:

```bash
premake5 vs2022
```

Then open the generated Visual Studio solution and build either:

```text
Debug
```

or:

```text
Release
```

The project is configured for the **x64 architecture**.

## Why I Built This

I built this project to understand regular expressions beyond simply using an existing library.

Implementing parts of a regex engine requires solving many of the same problems that appear in compilers and programming languages: parsing input, representing syntax, handling operators, and transforming text into structures that a program can evaluate.

It was also an opportunity to improve my understanding of C++ design, memory management, parsing, and low-level software development.

## Goals

The main goals of this project are:

* Learn how regular expression engines work internally
* Practice parser design in C++
* Explore compiler-related concepts
* Build complex syntax structures from raw text
* Improve my understanding of modern C++ and systems programming

## Technologies

* **C++**
* **Premake5**
* **Visual Studio / MSVC**

## Status

This is primarily an educational and experimental implementation rather than a replacement for production regex libraries such as `std::regex`, PCRE, or RE2.

Development is focused on understanding the architecture and algorithms behind parsing and evaluating regular expressions.

## Future Improvements

Possible future additions include:

* Expanded regex syntax support
* Better syntax error reporting
* Additional parser tests
* Pattern matching benchmarks
* More extensive documentation
* Regex visualization/debugging tools
* Performance improvements

## Author

**Akmal Mukhamadiev**

GitHub: [@akmalm07](https://github.com/akmalm07)
