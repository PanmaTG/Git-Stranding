---
favicon: https://github.com
---
**Link:** https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716
**Link:** https://medium.com/@noriller/docs-conventional-commits-feat-fix-refactor-which-is-which-531614fcb65a

---
# Rules
– Commit messages should always be in **lowercase**
– However, if there is a proper noun, that word should start with an **Uppercase** letter (If abbreviated, **all letters are capitalized**)
```code
fix(ui): correct GitHub badge alignment  
feat(api): add JWT authentication
```

# Format: 
– `<type>(<scope>): <subject>`
– `<scope>` is optional 
## Example
```
feat: add hat wobble
^--^  ^------------^
|     |
|     +-> Summary in present tense.
|
+-------> Type: chore, docs, feat, fix, refactor, style, or test.
```

---
# Types
## feat ↔ New functionality
— Use when you add behavior that didn’t exist before.
— If the user can now do something new → `feat`.
```bash
feat: add reply button
feat(auth): implement login validation
feat(api): support pagination
feat(ui): add dark mode toggle  
feat(search): implement keyword filtering
```

## fix ↔ Bug fix
— Use when something was broken and now works correctly.
— If you're correcting wrong behavior → `fix`.
```bash
fix(ui): correct reply button alignment  
fix(auth): prevent login crash on empty input  
fix(api): handle null response properly
fix(search): correct case-sensitive filtering bug
```

## refactor ↔ Code improvement, no behavior change
— Use when you restructure code but it behaves the same.
— If the app works the same before and after → `refactor`.
```bash
refactor(ui): simplify button component logic  
refactor(api): extract validation into helper function
refactor(auth): simplify validation conditions  
refactor: clean up unused variables
```

## docs ↔ Documentation only
— Use when you change README, comments, guides.
```bash
docs: update README installation steps  
docs: add usage example  
docs: correct typo in documentation
docs(api): add endpoint usage examples
```

## chore ↔ Maintenance / Setup
— Use for non-feature, non-bug tasks.
```bash
chore: add .gitignore  
chore: configure eslint  
chore: update dependencies  
chore: initial project setup
chore: rename folders for consistency
```

## style ↔
— For formatting only (no logic change).
```bash
style: format code with prettier
style: fix indentation in script.js  
style: remove trailing whitespace  
style(ui): adjust spacing in CSS file
```

## test ↔
— If you start writing tests:
```bash
test: add unit tests for login validation
test(auth): update validation tests for new password rules
test(api): fix failing pagination test  
test(ui): correct snapshot mismatch
```

## perf
— Performance improvements:
— Use only if performance specifically improved.
```bash
perf: optimize message rendering loop
perf(api): reduce redundant database queries  
perf(ui): debounce search input handler
```

## ci
— A commit of `ci` means changes related to Continuous Integration (usually `yml` and other configuration files).
```bash
ci: add GitHub Actions workflow  
ci: fix failing CI pipeline  
ci: update test workflow configuration  
ci: add Node.js version matrix
```

## build
—  A commit of `build` means changes related to the build of the project and dependencies. (Basically, anything that can change the build step of the application.)
```bash
build: update webpack configuration  
build: upgrade TypeScript to v5  
build: modify Vite config for alias support  
build: update Dockerfile setup
```