# awesome-phel [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome [Phel](https://phel-lang.org/) libraries, tools, projects, and resources.

[Phel](https://phel-lang.org/) is a functional, Lisp-inspired language that compiles to PHP. Persistent data structures, macros, and Clojure-style idioms on top of the PHP ecosystem.

## Contents

- [Core](#core)
- [Editor / IDE Plugins](#editor--ide-plugins)
- [Project Skeletons](#project-skeletons)
- [Libraries](#libraries)
  - [CLI](#cli)
  - [Database](#database)
  - [Validation](#validation)
- [Projects & Apps](#projects--apps)
  - [Games](#games)
  - [Web Apps](#web-apps)
  - [Utilities & Demos](#utilities--demos)
- [Articles & Blog Posts](#articles--blog-posts)
- [Community](#community)
- [Contributing](#contributing)

## Core

- [phel-lang](https://github.com/phel-lang/phel-lang) - The Phel language compiler and runtime.
- [phel-lang.org](https://github.com/phel-lang/phel-lang.org) - Official Phel website source.
- [clojure-test-suite](https://github.com/phel-lang/clojure-test-suite) - Clojure test suite support for Phel.

## Editor / IDE Plugins

- [phel-vs-code-extension](https://github.com/phel-lang/phel-vs-code-extension) - VS Code extension for Phel.
- [phel-intellij-plugin](https://github.com/phel-lang/phel-intellij-plugin) - Official IntelliJ / PhpStorm plugin.

## Project Skeletons

- [web-skeleton](https://github.com/phel-lang/web-skeleton) - Skeleton for building a website with Phel.
- [cli-skeleton](https://github.com/phel-lang/cli-skeleton) - Skeleton for building a CLI app with Phel.

## Libraries

### CLI

- [phel-cli-gui](https://github.com/Chemaclass/phel-cli-gui) - Functions to render UI in the terminal.
- [phel-getopt](https://github.com/smeghead/phel-getopt) - Command-line argument parsing for Phel CLI programs.

### Database

- [phel-pdo](https://github.com/phel-lang/phel-pdo) - PDO wrapper for database interaction.

### Validation

- [phel-schema](https://github.com/phel-lang/phel-schema) - Schema validation library inspired by [zod](https://zod.dev/).

## Projects & Apps

### Games

- [phel-snake](https://github.com/Chemaclass/phel-snake) - Snake game for the CLI terminal.
- [phel-tic-tac-toe](https://github.com/smeghead/phel-tic-tac-toe) - Tic-tac-toe in the terminal.
- [phel-lifegame](https://github.com/smeghead/phel-lifegame) - Conway's Game of Life simulation.
- [phel-cellular-automaton](https://github.com/smeghead/phel-cellular-automaton) - Cellular automaton simulation.
- [phelgeon](https://github.com/Lacsw/phelgeon) - Community Phel project (game/experiment).

### Web Apps

- [mariobasic-n7](https://github.com/mabasic/mariobasic-n7) - Personal website built in Phel.
- [phel-old-school-guestbook](https://github.com/smeghead/phel-old-school-guestbook) - Old-school message board with MySQL backend.
- [lisp-webscript-examples](https://github.com/kloimhardt/lisp-webscript-examples) - Web apps combining Phel with ClojureScript via GraphQL.

### Utilities & Demos

- [zo3ja](https://github.com/smeghead/zo3ja) - CLI RSS feed checker.
- [phel-saraudon](https://github.com/smeghead/phel-saraudon) - Git log visualization utility.
- [phel-mml2wav](https://github.com/smeghead/phel-mml2wav) - WAV file generation from MML notation.

## Articles & Blog Posts

- [Destructuring Deep Dive in Phel](https://phel-lang.org/blog/destructuring-deep-dive/) - Nested vectors/maps, `:keys`, `:or`, `:as`, `& rest`, JSON payloads.
- [Writing Your First Macro in Phel](https://phel-lang.org/blog/writing-your-first-macro/) - Step-by-step intro to macros.
- [Pattern Matching: Writing Cleaner Code with Less Conditional Logic](https://phel-lang.org/blog/pattern-matching/) - `case` and `cond` over `if/elseif` chains.
- [Immutability in Phel: Why Your Data Should Never Change](https://phel-lang.org/blog/immutability-in-phel/) - Persistent data structures and predictable code.
- [Threading Macros: Thread-First vs. Thread-Last](https://phel-lang.org/blog/threading-macros/) - Readable data pipelines.
- [Loop and Recur: Tail-Recursive Iteration Made Easy](https://phel-lang.org/blog/loop-and-recur/) - Tail recursion without losing clarity.
- [Map, Filter, Reduce: Your First Functional Toolkit in Phel](https://phel-lang.org/blog/map-filter-reduce/) - Functional fundamentals with REPL examples.
- [Functional Programming in PHP: Lessons from My First Experiments](https://phel-lang.org/blog/functional-programming-in-php/) - Early FP exploration that influenced Phel.

## Community

- [Official Website](https://phel-lang.org/)
- [Getting Started](https://phel-lang.org/documentation/getting-started/)
- [API Reference](https://phel-lang.org/documentation/reference/api/)
- [Practice Exercises](https://phel-lang.org/practice)
- [Contributing Guide](https://github.com/phel-lang/phel-lang/blob/main/.github/CONTRIBUTING.md)

## Contributing

PRs welcome. Add new entries in alphabetical order within their section. 

> Each entry: `- [name](url) - short description ending with a period.`
