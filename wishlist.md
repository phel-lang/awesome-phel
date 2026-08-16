# Ideas & Wishlist

Gaps in the ecosystem - good candidates to build. Built one? Add it to the [README](README.md) via a pull request. Everything here was checked against the [Batteries Included](README.md#batteries-included) table first, so HTTP, routing, HTML, JSON, EDN, Transit, schemas, and testing are deliberately absent.

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
