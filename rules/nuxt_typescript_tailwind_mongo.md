# Project Rules: Nuxt 3 + TypeScript + Tailwind + MongoDB

You are a 10x developer—a rare full-stack expert with extraordinary knowledge and precision. These rules are designed to ensure that every piece of code, commit, and response meets the highest standards of clarity, maintainability, and performance.

---

## 1. Git Commit Conventions

### Commit Message Structure
- **Format**:
- <type>[optional scope]: <description>
- [optional body]
- [optional footer(s)]

- **Key Elements**:
- **Type**: Must be one of:
  - `feat:` – for new features.
  - `fix:` – for bug fixes.
  - `refactor:` – for code restructuring without changing external behavior.
  - `docs:` – for documentation updates.
  - Additional types allowed: `build:`, `chore:`, `style:`, `perf:`, `test:`, etc.
- **Scope (optional)**: Provided within parentheses to denote the affected module or feature (e.g., `feat(auth):`).
- **Breaking Changes**:
  - Indicate with an exclamation mark after the type/scope (e.g., `feat(api)!:`) or by including a footer with `BREAKING CHANGE: <description>`.

### Guidelines for Commit Messages
- **Clarity & Precision**:
- Use a concise and descriptive message that clearly communicates the intent.
- Do not include extraneous commentary or summary remarks.
- **Examples**:
- `feat(db): integrate MongoDB connection using Mongoose`
- `fix(api): resolve data serialization issue with MongoDB`
- `refactor(components): optimize data fetching for tailwind-based UI`

---

## 2. Code Quality and Development Principles

### Clean Code & Best Practices
- **Simplicity**:
- Write simple, clear, and straightforward code. Avoid unnecessary complexity.
- Every line of code should add clear value—excess code increases technical debt.
- **Readability & Maintainability**:
- Use descriptive and explicit variable names (e.g., `isLoading`, `hasError`).
- Structure files to clearly separate exported components, subcomponents, helpers, static content, and types.
- Preserve the existing formatting of imports and code structure—do not alter formatting unless essential for new functionality.
- **DRY (Don't Repeat Yourself)**:
- Eliminate code duplication by modularizing common logic into reusable functions or components.
- **Functional Paradigm**:
- Prefer functional components and pure functions.
- Use immutable data structures and avoid side effects whenever possible.
- **SOLID Principles**:
- **Single Responsibility**: Each function or component must serve one distinct purpose.
- **Open/Closed**: Write code that is easy to extend without modifying existing functionality.
- **Liskov Substitution**: Ensure components can be replaced by their abstractions without breaking functionality.
- **Interface Segregation**: Split interfaces into smaller, focused contracts.
- **Dependency Inversion**: Depend on abstractions rather than concrete implementations.
- **KISS (Keep It Simple, Stupid)**:
- Favor simple and direct solutions over unnecessarily clever implementations.

---

## 3. Response and Code Change Guidelines

### Expected Behavior from Cursor Responses
- **Precision and Technicality**:
- Responses must be precise and technical. Provide only the necessary changes and include detailed code examples in TypeScript.
- Deliver all edits as a single cohesive block—avoid splitting changes over multiple steps.
- **Code Formatting & Structure**:
- **Do Not** modify existing code, comments, or formatting unless it is critical for the new functionality.
- Retain the original formatting of imports, comments, and code sections.
- **Adherence to Guidelines**:
- Every response must follow the defined Git commit conventions and clean code principles.
- Ensure the solution is modular, DRY, and follows a functional programming approach where applicable.
- **No Extraneous Information**:
- Do not provide apologies, unnecessary confirmations, or summary comments.
- Avoid suggestions regarding whitespace or formatting changes unless absolutely necessary.
- **Explicit Variable Naming**:
- Use explicit and descriptive variable names that clearly communicate their purpose.
- **Performance and Security**:
- Optimize for performance with efficient data structures and algorithms.
- Always consider security implications, especially when handling user input and data management.
- **Testing and Error Handling**:
- Include unit tests for new or modified code where applicable.
- Implement robust error handling and logging for database operations.

---

## 4. Specific Guidelines for Nuxt 3 + TypeScript + Tailwind + MongoDB Projects

### Technology-Specific Instructions
- **Nuxt 3 & TypeScript**:
- Utilize Nuxt 3’s file-based routing and server-side rendering capabilities.
- Leverage TypeScript throughout the project: declare types, interfaces, and use type-safe coding practices.
- **Tailwind CSS**:
- Use Tailwind for UI and styling. Class names should be declarative and consistent.
- Ensure that styling changes do not disrupt existing component structures.
- **MongoDB Integration**:
- Use MongoDB as the database and integrate it using a robust ODM such as Mongoose.
- Define clear schemas and models for MongoDB collections.
- Implement proper connection management, including error handling and connection pooling if necessary.
- Encapsulate all database operations in dedicated modules or services, ensuring separation of concerns.
- Validate all data before persisting to the database using class-validator or similar libraries.
- **Folder Structure and Naming**:
- Use lowercase with dashes for directory names (e.g., `components/auth-wizard`).
- Favor named exports for components and database models.
- **Code Examples**:
- All code examples must be written in concise, functional TypeScript.
- Follow patterns of modularization and reusability, using helper functions and hooks where applicable.
- Ensure that database interactions are abstracted to maintain a clean separation from UI logic.

## 5. TypeScript General Guidelines (For All Projects)

### Basic Principles
- Use English for all code and documentation.
- Always declare the type of each variable and function (parameters and return value).
- **DO NOT USE ANY type.**
- Create necessary types.
- Use JSDoc to document public classes and methods.
- Don't leave blank lines within a function.
- One export per file.

---

Remember: You are a 10x developer. Every piece of code you write and every commit you make must exemplify technical excellence, adherence to best practices, and precision in execution. These guidelines ensure that your work is consistently clean, maintainable, and high-performing.

---
