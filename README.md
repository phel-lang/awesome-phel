# Awesome Phel [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome Phel libraries, tools, projects, and resources.

Phel is a functional, Lisp-inspired language that compiles to PHP: persistent data structures, macros, and Clojure-style idioms on top of the PHP ecosystem.

## Contents

- [Core](#core)
- [Batteries Included](#batteries-included)
- [Editor / IDE Plugins](#editor--ide-plugins)
- [Tooling](#tooling)
- [Project Skeletons](#project-skeletons)
- [Packages & Libraries](#packages--libraries)
  - [CLI](#cli)
  - [Database](#database)
  - [Logging](#logging)
  - [Validation](#validation)
- [Projects & Apps](#projects--apps)
  - [Games](#games)
  - [Web Apps](#web-apps)
  - [Integrations](#integrations)
  - [Utilities & Demos](#utilities--demos)
- [Learning](#learning)
  - [Tutorials & Deep Dives](#tutorials--deep-dives)
  - [Release Notes](#release-notes)
- [Community](#community)
- [Ideas & Wishlist](#ideas--wishlist)

## Core

- [clojure-test-suite](https://github.com/phel-lang/clojure-test-suite) - Clojure test suite support for Phel.
- [phel-lang](https://github.com/phel-lang/phel-lang) - The Phel language compiler and runtime.
- [phel-lang.org](https://github.com/phel-lang/phel-lang.org) - Official Phel website source.

## Batteries Included

Namespaces shipped with the compiler - check here before reaching for a library or building one. Full signatures live in the API reference linked under Community.

| Namespace          | What it covers                                                                  |
| ------------------ | ------------------------------------------------------------------------------- |
| `phel.ai`          | Helpers for talking to LLM providers from Phel                                  |
| `phel.async`       | Promises, futures, fibers, `pmap`, `await` / `await-all` / `await-any`          |
| `phel.base64`      | Base64 and URL-safe Base64 encoding                                             |
| `phel.cli`         | Argument parsing, option coercion, command dispatch                             |
| `phel.edn`         | Read and write EDN                                                              |
| `phel.html`        | Hiccup-style HTML generation from vectors and maps                              |
| `phel.http`        | URI, request, and response values plus PSR-7 bridging                           |
| `phel.http-client` | HTTP requests over a pluggable client                                           |
| `phel.json`        | JSON encode/decode into Phel data structures                                    |
| `phel.match`       | Structural pattern matching macro                                               |
| `phel.mock`        | Test doubles with a mock registry                                               |
| `phel.pprint`      | Pretty-printing of nested data                                                  |
| `phel.reader`      | Tagged-literal registry (`#foo value`)                                          |
| `phel.reflect`     | PHP reflection returning Phel collections                                       |
| `phel.repl`        | REPL utilities, namespace reloading, `doc`, `require`                           |
| `phel.router`      | Routing built on the Symfony routing component                                  |
| `phel.schema`      | Data-driven schemas: validation, coercion, explain, generation, instrumentation |
| `phel.string`      | String utilities                                                                |
| `phel.test`        | Test framework with structural diffs and reporting                              |
| `phel.trace`       | Function-call tracing in the spirit of `clojure.tools.trace`                    |
| `phel.transit`     | Read and write Transit+JSON-Verbose                                             |
| `phel.walk`        | Generic tree walking (`prewalk`, `postwalk`)                                    |
| `phel.watch`       | React to file changes from within Phel                                          |

The CLI ships more than a compiler: `run`, `repl`, `eval`, `test`, `build`, `format`, `lint`, `analyze`, `doc`, `doctor`, `config`, `watch`, `profile`, `export`, `init`, `nrepl`, and `lsp`.

## Editor / IDE Plugins

- [phel-intellij-plugin](https://github.com/phel-lang/phel-intellij-plugin) - Official IntelliJ / PhpStorm plugin.
- [phel-vs-code-extension](https://github.com/phel-lang/phel-vs-code-extension) - VS Code extension: highlighting, completion, hover, diagnostics, REPL, paredit, refactoring, Xdebug adapter.

## Tooling

- [phel-nrepl](https://github.com/leobm/phel-nrepl) - nREPL server for Phel, for use with Calva and other nREPL clients.
- [setup-phel-action](https://github.com/phel-lang/setup-phel-action) - Set up Phel in GitHub Actions workflows.

## Project Skeletons

- [cli-skeleton](https://github.com/phel-lang/cli-skeleton) - Skeleton for building a CLI app with Phel.
- [phel-web-skeleton](https://github.com/leobm/phel-web-skeleton) - Web starter with dev server, auto-build, and error overlays.
- [web-skeleton](https://github.com/phel-lang/web-skeleton) - Skeleton for building a website with Phel.

## Packages & Libraries

### CLI

- [phel-cli-gui](https://github.com/Chemaclass/phel-cli-gui) - Functions to render UI in the terminal.
- [phel-getopt](https://github.com/smeghead/phel-getopt) - Command-line argument parsing for Phel CLI programs.

### Database

- [phel-pdo](https://github.com/phel-lang/phel-pdo) - PDO wrapper for database interaction.
- [phel-sql](https://github.com/phel-lang/phel-sql) - Data-driven SQL DSL inspired by HoneySQL. Pure data in, `[sql params]` out.

### Logging

- [phel-log](https://github.com/phel-lang/phel-log) - Data-driven logging with levels, namespace filtering, pluggable appenders, a PSR-3 adapter, and a Monolog handler bridge. Inspired by Timbre + Monolog.

### Validation

- [phel-schema](https://github.com/phel-lang/phel-schema) - Standalone schema validation library inspired by [zod](https://zod.dev/).

## Projects & Apps

### Games

- [phel-cellular-automaton](https://github.com/smeghead/phel-cellular-automaton) - Cellular automaton simulation.
- [phel-connect4](https://github.com/Chemaclass/phel-connect4) - Two-player terminal Connect 4 with an optional bitboard minimax AI.
- [phel-doom](https://github.com/Chemaclass/phel-doom) - DOOM-lite raycaster with 256-color ANSI and procedural levels.
- [phel-flappybird](https://github.com/Chemaclass/phel-flappybird) - Flappy Bird in the CLI terminal.
- [phel-lifegame](https://github.com/smeghead/phel-lifegame) - Conway's Game of Life simulation.
- [phel-snake](https://github.com/Chemaclass/phel-snake) - Snake game for the CLI terminal.
- [phel-tic-tac-toe](https://github.com/smeghead/phel-tic-tac-toe) - Tic-tac-toe in the terminal.
- [phelgeon](https://github.com/Lacsw/phelgeon) - Procedural, turn-based dungeon crawler for the terminal.

### Web Apps

- [lisp-webscript-examples](https://github.com/kloimhardt/lisp-webscript-examples) - Web apps combining Phel with ClojureScript via GraphQL.
- [mariobasic-n7](https://github.com/mabasic/mariobasic-n7) - Personal website built in Phel.
- [phel-old-school-guestbook](https://github.com/smeghead/phel-old-school-guestbook) - Old-school message board with MySQL backend.

### Integrations

- [phel-symfony-demo](https://github.com/Chemaclass/phel-symfony-demo) - Symfony + Phel: Ring-style handlers over plain maps, no ORM, ~90 LOC adapter.
- [wp-http-eval](https://github.com/jasalt/wp-http-eval) - WordPress plugin evaluating Phel expressions from the admin dashboard or a token-authenticated REST endpoint.

### Utilities & Demos

- [phel-crawler](https://github.com/SauronBot/phel-crawler) - Web crawler CLI using Guzzle and Symfony DomCrawler.
- [phel-mml2wav](https://github.com/smeghead/phel-mml2wav) - WAV file generation from MML notation.
- [phel-saraudon](https://github.com/smeghead/phel-saraudon) - Git log visualization utility.
- [zo3ja](https://github.com/smeghead/zo3ja) - CLI RSS feed checker.

## Learning

### Tutorials & Deep Dives

Newest first.

- [PHP Interop in Phel: Modern Syntax](https://phel-lang.org/blog/php-interop-modern-syntax/) - Named arguments, by-reference output, magic methods, typed wrappers, native enums.
- [REPL-Driven Development in Phel](https://phel-lang.org/blog/repl-driven-development/) - Live functions, `*1` chaining, `load-file` reloads, `tap>` debugging.
- [Destructuring Deep Dive in Phel](https://phel-lang.org/blog/destructuring-deep-dive/) - Nested vectors/maps, `:keys`, `:or`, `:as`, `& rest`, JSON payloads.
- [Writing Your First Macro in Phel](https://phel-lang.org/blog/writing-your-first-macro/) - Step-by-step intro to macros.
- [Pattern Matching: Writing Cleaner Code with Less Conditional Logic](https://phel-lang.org/blog/pattern-matching/) - `case` and `cond` over `if/elseif` chains.
- [Immutability in Phel: Why Your Data Should Never Change](https://phel-lang.org/blog/immutability-in-phel/) - Persistent data structures and predictable code.
- [Threading Macros in Phel: Thread-First vs. Thread-Last](https://phel-lang.org/blog/threading-macros/) - Readable data pipelines.
- [Loop and Recur: Tail-Recursive Iteration Made Easy](https://phel-lang.org/blog/loop-and-recur/) - Tail recursion without losing clarity.
- [Map, Filter, Reduce: Your First Functional Toolkit in Phel](https://phel-lang.org/blog/map-filter-reduce/) - Functional fundamentals with REPL examples.
- [Functional Programming in PHP: Lessons from My First Experiments](https://phel-lang.org/blog/functional-programming-in-php/) - Early FP exploration that influenced Phel.

### Release Notes

- [Phel 0.47: Clear Signals](https://phel-lang.org/blog/phel-0-47-clear-signals/) - LSP signature help, per-session REPL value history over nREPL, examples in `(doc)`, structural test diffs, ~30% faster startup.
- [Phel 0.46: Native Path](https://phel-lang.org/blog/phel-0-46-native-path/) - Config validation in `phel doctor`, per-phase build timing, honest build exit codes, cascading incremental cache.

## Community

- [Official Website](https://phel-lang.org/)
- [Getting Started](https://phel-lang.org/documentation/getting-started/)
- [API Reference](https://phel-lang.org/documentation/reference/api/)
- [Practice Exercises](https://phel-lang.org/practice)
- [Blog](https://phel-lang.org/blog/)
- [Contributing Guide](https://github.com/phel-lang/phel-lang/blob/main/.github/CONTRIBUTING.md)

## Ideas & Wishlist

Gaps in the ecosystem - good candidates to build. Everything here was checked against the Batteries Included table first, so HTTP, routing, HTML, JSON, EDN, Transit, schemas, and testing are deliberately absent.

**Data & Serialization**

- CSV reader/writer, streaming-friendly (league/csv, `clojure.data.csv`)
- YAML parser (Symfony YAML, clj-yaml)
- Markdown parser and renderer to Hiccup-style data (commonmark)
- Spreadsheet reader/writer (PhpSpreadsheet)
- Zipper API for navigating and editing nested trees (`clojure.zip`)
- Query/transform DSL over nested data (specter, meander)
- Parser combinators or a grammar DSL (instaparse)

**Application Building Blocks**

- Date/time library over `DateTimeImmutable` (Carbon, tick)
- Environment and config loading with validation (phpdotenv, aero)
- Dependency/state lifecycle management (integrant, mount)
- Event dispatcher and pub/sub (Symfony EventDispatcher)
- UUID / ULID generation (ramsey/uuid)
- Money and arbitrary-precision decimal math (moneyphp)
- i18n and translation catalogs (Symfony Translation, tongue)
- Caching abstraction over PSR-6 / PSR-16 (`core.cache`)
- Redis client with data-first API (carmine)
- Queue and background job worker (Symfony Messenger)
- Mailer with template rendering (Symfony Mailer)
- Filesystem abstraction across local/S3 (Flysystem)
- Sessions, authentication, and password hashing helpers
- Rate limiter and circuit breaker middleware
- Feature flags with runtime overrides

**Web**

- Minimal web framework on top of `phel.router` - middleware stack, Ring-style handlers (Ring + Compojure, Slim)
- htmx helpers producing `phel.html` fragments
- OpenAPI spec generation from `phel.schema` definitions (reitit-swagger)
- WebSocket / SSE server
- CSRF, CORS, and security-header middleware

**Tooling**

- Idiom and style rules layered on `phel lint` (clj-kondo's linters as a rule pack)
- Property-based testing generators on top of `phel.schema` (test.check)
- Benchmarking harness with statistical output on top of `phel profile` (criterium)
- Code coverage reporting for `.phel` files, Codecov-ready
- Database migrations runner (migratus, Phinx)
- Dependency graph and dead-code visualizer
- Error tracking adapter (Sentry, Bugsnag)
- Official Docker images with the compiler and PHAR preinstalled
- Reusable CI workflow wrapping `phel format`, `phel lint`, and `phel test`
- MCP server written in Phel, exposing project tools over `phel.ai`

**Projects & Apps**

- Static site generator with Hiccup templates and Markdown content
- Blog engine (Luminus, Sculpin)
- REST API starter kit with auth, validation, and OpenAPI (Mezzio, Pedestal)
- Admin panel generator driven by schemas (Filament, Nova)
- CLI task runner (Robo, Task)
- TUI framework beyond phel-cli-gui - components, layout, event loop (bubbletea)
- Laravel package and a real Symfony bundle, not just a demo
- Discord or Telegram bot framework

**Community & Learning**

- Browser playground running Phel on php-wasm
- Exercism track for Phel
- "Phel by Example" cookbook site with runnable snippets
- Package catalog listing Phel-specific Packagist releases
- Advent of Code solutions repository

## Contributing

Contributions welcome! Read the [contribution guidelines](contributing.md) first.
