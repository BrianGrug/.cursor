# General Rules

This set of guidelines ensures consistency, clarity, performance, and maintainability across all languages and projects. Always apply these principles to produce clean, understandable, and efficient code.

Make SURE you use your MCP tools. They are very powerful, and will help you remember things, search for things, get my logs for me, and more. Make sure you use MCP tools as often as you possibly can.

## Code Style and Readability

1. **Clarity Over Brevity**:
   - Favor understandable code over clever tricks.
   - Prioritize legibility and maintainability over saving a few lines.
2. **Consistent Naming Conventions**:
   - Use descriptive, self-explanatory names for variables, functions, classes, and modules.
   - Follow language-specific naming conventions (e.g., `snake_case` for Python, `camelCase` for JavaScript) and remain consistent throughout the codebase.
3. **Consistent Formatting**:
   - Adhere to a uniform indentation style, spacing, and line width.
   - Use automated tools (linters, formatters) to enforce consistency and reduce manual overhead.
4. **Comments That Add Value**:
   - Write comments to explain the "why" behind complex logic, not just the "what."
   - Remove or avoid redundant comments that restate the obvious.
5. **Small, Single-Responsibility Functions**:
   - Keep functions concise and focused on doing one thing well.
   - Break larger functionalities into smaller, reusable units that are easier to test and maintain.

## Architecture and Modularity

1. **Encapsulation of Complexity**:
   - Hide complex logic behind clear interfaces or modules.
   - Present a simple, well-documented API to callers while keeping internals flexible and interchangeable.
2. **Decouple Components**:
   - Design modules with minimal direct knowledge of each other's implementations.
   - Use inheritance, ensure reusable and improve testability and flexibility.
3. **DRY (Don't Repeat Yourself)**:
   - Factor out repetitive patterns into shared functions or classes.
   - Refactor early and often to prevent code drift and bloat over time.

## Error Handling and Testing

1. **Fail Fast, Fail Loud**:
   - Validate assumptions early, return or throw errors as soon as something unexpected happens.
   - Provide clear error messages that help identify the root cause quickly.
2. **Testability as a Priority**:
   - Write code that is easy to test in isolation.
   - Separate pure logic from side effects, use inheritance, and ensure complex logic resides in testable units.
3. **Thorough Input Validation**:
   - Check all inputs for correctness, sanity, and security risks before processing.
   - Guard against malformed data, null references, or out-of-bound values.

## Performance and Resource Management

1. **Appropriate Data Structures and Algorithms**:
   - Choose data structures and algorithms best suited for the problem to ensure reasonable time and space complexity.
   - Opt for clarity first, and only optimize further if and when performance profiling indicates a need.
2. **Avoid Premature Optimization**:
   - Start with a clean, readable solution.
   - Measure performance with profiling tools and address hotspots instead of guessing where optimization is needed.
3. **Resource Lifecycle Awareness**:
   - Properly manage memory, file handles, network connections, and other resources.
   - Use language-specific best practices (e.g., RAII, `with` statements, finally blocks) to ensure proper cleanup.

# Commit Message Guidelines

## Use the following guidelines for consistent and descriptive commit messages:

## prefix: short description (maximum one sentence)

Commit Prefixes:

- feat: Introduce a new feature.
- fix: Fix a bug or issue.
- tweak: Make minor adjustments or improvements.
- style: Update code style or formatting.
- refactor: Restructure code without changing functionality.
- perf: Improve performance or efficiency.
- test: Add or update tests.
- docs: Update documentation.
- chore: Perform maintenance tasks or updates.
- ci: Change CI/CD configuration.
- build: Modify build system or dependencies.
- revert: Revert a previous commit.
- hotfix: Apply an urgent bug fix.
- init: Initialize a new project or feature.
- merge: Merge branches.
- wip: Mark work in progress.
- release: Prepare for a release.
