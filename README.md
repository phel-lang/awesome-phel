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
  - [Data & Serialization](#data--serialization)
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
  - [Articles](#articles)
  - [Talks & Videos](#talks--videos)
  - [Examples & Katas](#examples--katas)
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
- [phel-mode](https://github.com/jasalt/phel-mode) - Emacs major mode based on clojure-mode, with REPL workflow and in-progress LSP / CIDER support.
- [phel-vs-code-extension](https://github.com/phel-lang/phel-vs-code-extension) - VS Code extension: highlighting, completion, hover, diagnostics, REPL, paredit, refactoring, Xdebug adapter.
- [phel.vim](https://github.com/danirod/phel.vim) - Vim syntax highlighting and filetype detection for `.phel` files.

## Tooling

- [Docker image `phellang/repl`](https://hub.docker.com/r/phellang/repl) - Official image to start a Phel REPL with `docker run -it --rm phellang/repl`.
- [nixpkgs `phel`](https://github.com/NixOS/nixpkgs/blob/master/pkgs/by-name/ph/phel/package.nix) - Phel packaged for Nix, `nix shell nixpkgs#phel`.
- [phel-nrepl](https://github.com/leobm/phel-nrepl) - nREPL server for Phel, for use with Calva and other nREPL clients.
- [phel-nrepl (jasalt)](https://codeberg.org/jasalt/phel-nrepl) - nREPL server written in Phel on amphp/socket, with Emacs / CIDER and Calva setup notes.
- [setup-phel-action](https://github.com/phel-lang/setup-phel-action) - Set up Phel in GitHub Actions workflows.

## Project Skeletons

- [cli-skeleton](https://github.com/phel-lang/cli-skeleton) - Skeleton for building a CLI app with Phel.
- [phel-web-skeleton](https://github.com/leobm/phel-web-skeleton) - Web starter with dev server, auto-build, and error overlays.
- [web-skeleton](https://github.com/phel-lang/web-skeleton) - Skeleton for building a website with Phel.

## Packages & Libraries

### CLI

- [phel-cli-gui](https://github.com/Chemaclass/phel-cli-gui) - Functions to render UI in the terminal.
- [phel-getopt](https://github.com/smeghead/phel-getopt) - Command-line argument parsing for Phel CLI programs.

### Data & Serialization

- [phel-bencode](https://gitlab.com/jasalt/phel-bencode) - Bencode encoding and decoding of Phel data structures, on Packagist as `jasalt/phel-bencode`.

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
- [phel-minesweeper](https://github.com/SauronBot/phel-minesweeper) - Terminal Minesweeper with flagging, four difficulty levels, and a safe first click.
- [phel-snake](https://github.com/Chemaclass/phel-snake) - Snake game for the CLI terminal.
- [phel-tic-tac-toe](https://github.com/smeghead/phel-tic-tac-toe) - Tic-tac-toe in the terminal.
- [phelgeon](https://github.com/Lacsw/phelgeon) - Procedural, turn-based dungeon crawler for the terminal.

### Web Apps

- [lisp-webscript-examples](https://github.com/kloimhardt/lisp-webscript-examples) - Web apps combining Phel with ClojureScript via GraphQL.
- [mariobasic-n7](https://github.com/mabasic/mariobasic-n7) - Personal website built in Phel.
- [phel-old-school-guestbook](https://github.com/smeghead/phel-old-school-guestbook) - Old-school message board with MySQL backend.

### Integrations

- [demo-phel-datastar](https://github.com/jasalt/demo-phel-datastar) - Datastar hypermedia demo driven by server-sent events from Phel, with minimal JavaScript.
- [phel-google-sheets-example](https://codeberg.org/jasalt/phel-google-sheets-example) - Read and write Google Sheets from Phel via the Google API PHP client.
- [phel-symfony-demo](https://github.com/Chemaclass/phel-symfony-demo) - Symfony + Phel: Ring-style handlers over plain maps, no ORM, ~90 LOC adapter.
- [phel-wp-plugin](https://github.com/jasalt/phel-wp-plugin) - WordPress plugin skeleton rendering admin widgets with `phel.html`, with a devenv / Docker development setup.
- [phelano](https://github.com/leocavalcante/phelano) - Phel running on Hyperf's Nano coroutine HTTP server.
- [wp-http-eval](https://github.com/jasalt/wp-http-eval) - WordPress plugin evaluating Phel expressions from the admin dashboard or a token-authenticated REST endpoint.

### Utilities & Demos

- [Geo3x3](https://github.com/taisukef/Geo3x3) - Geocoding system implemented in 100+ languages, including a Phel port.
- [habit-tracker](https://github.com/JesusValeraDev/habit-tracker) - Command-line habit tracker with JSON persistence and streak tracking.
- [phel-aa](https://github.com/smeghead/phel-aa) - Convert PNG images into ASCII art from the command line.
- [phel-crawler](https://github.com/SauronBot/phel-crawler) - Web crawler CLI using Guzzle and Symfony DomCrawler.
- [phel-grep](https://github.com/smeghead/phel-grep) - Grep-like CLI built on phel-getopt.
- [phel-junkshed](https://github.com/jasalt/phel-junkshed) - Grab-bag of reusable Phel namespaces: CLI options, HTTP client, PDO, sitemap, WordPress and API helpers.
- [phel-mml2wav](https://github.com/smeghead/phel-mml2wav) - WAV file generation from MML notation.
- [phel-saraudon](https://github.com/smeghead/phel-saraudon) - Git log visualization utility.
- [phel-todo](https://github.com/CosmeValera/phel-todo) - Command-line todo manager exercising records, protocols, multimethods, and transducers.
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

### Articles

Third-party and off-site writing about Phel, newest first.

- [Exploring Programming Languages: Phel](https://blog.devgenius.io/exploring-programming-languages-phel-db3511d40be3) - Hands-on first contact with Phel, building a small LED-numbers app (2025).
- [Phel Lang, a native LISP for PHP](https://24daysindecember.net/2022/12/17/introduction-phel-lang-a-native-lisp-for-php/) - Advent-calendar introduction on 24 Days in December (2022).
- [Phel: the Lisp that compiles to PHP](https://dev.to/chemaclass/phel-the-lisp-that-compiles-to-php-963) - Early walkthrough of the language and its motivation on DEV (2021).
- [Phel Language, Lisp for PHP](https://phpmagazine.net/2021/01/phel-language-lisp-for-php.html) - PHP Magazine coverage of the first public releases (2021).

### Talks & Videos

Newest first.

- [Running DOOM in PHP with Phel](https://phpconference.com/php-core-coding/running-doom-php-phel/) - International PHP Conference, Munich (2026). [Slides](https://chemaclass.com/slides/phel-doom/).
- [Writing Lisp in PHP: A Journey with Phel](https://phpconference.com/php-core-coding/lisp-in-php-phel/) - International PHP Conference, Berlin (2026).
- [From $this to (this): A Gentle Introduction to Phel](https://phpconference.com/web-development/phel-introduction-functional-programming-lisp/) - International PHP Conference, Munich (2025).
- [Phel, a native Lisp for PHP](https://www.wearedevelopers.com/en/videos/791/phel-a-native-lisp-for-php) - WeAreDevelopers World Congress, Berlin (2023). Video, ~15 min.
- [Phel in 5 min](https://youtu.be/ZQTann9ItH8) - Berlin Hack & Tell lightning talk (2023). Video.
- [Phel Language: ¿Programación funcional para PHP?](https://www.youtube.com/live/9pElbTEcyGA) - DesarrolloWeb live session, in Spanish (2022). Video.
- [All Phel talks](https://chemaclass.com/talks/phel/) - Running index of conference and meetup talks about Phel.

### Examples & Katas

- [katas-phel](https://github.com/danirod-live/katas-phel) - Programming katas solved in Phel, from a Spanish-language live-coding stream.
- [phel-amphp-examples](https://github.com/jasalt/phel-amphp-examples) - AMPHP concurrency examples translated to Phel: fibers, socket servers, SSE, parallel functions.

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
- [GitHub Discussions](https://github.com/phel-lang/phel-lang/discussions)
- [@phel_lang on X](https://x.com/phel_lang)
- [Hacker News: launch thread (2021)](https://news.ycombinator.com/item?id=26184044) - 81 points, 34 comments. See also the [v0.36 thread (2026)](https://news.ycombinator.com/item?id=48059761).
- [awesome-lisp-languages](https://github.com/dundalek/awesome-lisp-languages) and [awesome-lisp-family](https://github.com/damon-kwok/awesome-lisp-family) - Lisp-family catalogs that list Phel.
- [clojure-dialects-docs](https://github.com/clj-easy/clojure-dialects-docs) - Catalog of Clojure dialects with a dedicated Phel entry.

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
- GitHub Linguist support so `.phel` files get highlighting and language stats ([PR open](https://github.com/github-linguist/linguist/pull/6282))
- Homebrew formula and asdf / mise plugin
- tree-sitter grammar for Phel (Neovim, Helix, Zed)
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
- Listing in awesome-php and on Wikipedia's Lisp-family languages page

## Contributing

Contributions welcome! Read the [contribution guidelines](contributing.md) first.
