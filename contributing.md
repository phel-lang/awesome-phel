# Contribution Guidelines

Pull requests are welcome. Please open one entry per pull request.

## Adding an entry

- Add entries in **alphabetical order** within their section. Exceptions: *Tutorials & Deep Dives* and *Release Notes* go newest first.
- Format: `- [name](url) - short description ending with a period.`
- Use a single hyphen (`-`) as the separator between link and description.
- Keep descriptions to one line. Say what the project does, not how great it is.
- The entry must be about Phel, work with a current Phel release, and have a public repository or page.
- If a new section is needed, add it to the [Contents](README.md#contents) list too.

## Quality bar

- Prefer projects with a README explaining what they do and how to install/run them.
- Archived, abandoned, or work-in-progress projects are not listed, and may be removed once they stop working.
- Before adding a wishlist idea, check [Batteries Included](README.md#batteries-included) - much of what a Clojure or PHP developer expects from a library already ships with the compiler.

## Checks

Before opening the pull request:

- Verify every link returns HTTP 200.
- Run the awesome list linter:

```bash
npx awesome-lint
```
