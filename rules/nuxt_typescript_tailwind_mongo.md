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
- Write simple, clear, and straightforward code. Avoid unnecessary complexity and over-engineering.
- Each line of code must serve a clear purpose; superfluous code increases technical debt.
- **Readability & Maintainability**:
- Use descriptive and explicit variable names (e.g., `isLoading`, `hasError`).
- Organize your project files to clearly separate exported components, subcomponents, helpers, static content, and types.
- Preserve the original formatting of imports and existing code structure—avoid reformatting unless essential.
- **DRY (Don't Repeat Yourself)**:
- Modularize common logic into reusable functions or components to avoid code duplication.
- **Functional Paradigm**:
- Prefer functional components and pure functions over stateful logic where possible.
- Use immutable data structures and avoid side effects to ensure predictable behavior.
- **SOLID Principles**:
- **Single Responsibility**: Ensure that each function or component serves one distinct purpose.
- **Open/Closed**: Write code that is open for extension but closed for modification.
- **Liskov Substitution**: Components should be easily replaceable with their abstractions without breaking functionality.
- **Interface Segregation**: Create fine-grained interfaces to prevent clients from depending on methods they do not use.
- **Dependency Inversion**: Depend on abstractions rather than concrete implementations.
- **KISS (Keep It Simple, Stupid)**:
- Favor simple, direct solutions over overly clever or complex implementations.
- **Additional Details**:
- Always validate assumptions with tests.
- Focus on modularity and reusability, ensuring that each module can be maintained or replaced independently.

---

## 3. Response and Code Change Guidelines

### Expected Behavior from Cursor Responses
- **Precision and Technicality**:
- Provide responses that are precise and technical, with detailed code examples in TypeScript.
- Deliver all modifications as a single cohesive block, ensuring no step-by-step fragmentation.
- **Code Formatting & Structure**:
- **Do Not** modify existing code, comments, or formatting unless it is absolutely necessary for the new functionality.
- Retain the original formatting of imports, comments, and code sections to preserve context.
- **Adherence to Guidelines**:
- Every response must adhere to the defined Git commit conventions and the clean code principles outlined above.
- Ensure that solutions are modular, DRY, and leverage functional programming approaches wherever applicable.
- **No Extraneous Information**:
- Exclude unnecessary apologies, confirmations, or summary remarks that do not contribute to the solution.
- Avoid recommendations for whitespace or formatting changes unless such modifications are critical.
- **Explicit Variable Naming**:
- Use explicit and descriptive variable names that clearly communicate their purpose.
- **Performance and Security**:
- Optimize for performance by using efficient data structures, algorithms, and rendering strategies.
- Always consider security implications, especially when handling user input and data management.
- **Testing and Error Handling**:
- Incorporate unit tests for new or modified code where applicable.
- Implement robust error handling and logging, particularly for database operations and sensitive processes.
- **Additional Considerations**:
- Maintain separation of concerns; avoid mixing business logic with UI logic.
- All changes must be minimal and focused solely on the necessary modifications.

---

## 4. Specific Guidelines for Nuxt 3 + TypeScript + Tailwind + MongoDB Projects

### Technology-Specific Instructions
- **Nuxt 3 & TypeScript**:
- Utilize Nuxt 3’s file-based routing and server-side rendering capabilities to maximize performance.
- Leverage TypeScript throughout the project—ensure all types and interfaces are declared, enforcing type safety.
- **Tailwind CSS**:
- Use Tailwind for UI and styling. Class names should be declarative and consistent.
- Ensure styling changes integrate seamlessly without disrupting existing component structures.
- **MongoDB Integration**:
- Use MongoDB as the primary database and integrate it using a robust ODM such as Mongoose.
- Define clear, well-documented schemas and models for MongoDB collections.
- Implement proper connection management, including error handling and connection pooling if needed.
- Encapsulate all database operations within dedicated modules or services to maintain a clear separation of concerns.
- Validate all data before persisting it to the database using libraries such as class-validator.
- **Folder Structure and Naming**:
- Use lowercase with dashes for directory names (e.g., `components/auth-wizard`).
- Favor named exports for components and database models.
- **Code Examples**:
- All code examples must be written in concise, functional TypeScript.
- Follow modularization and reusability patterns, utilizing helper functions and hooks where applicable.
- Ensure that database interactions are abstracted from UI logic, maintaining a clean architectural separation.

---

## 5. TypeScript General Guidelines (For All Projects)

### Basic Principles
- Use English for all code and documentation.
- Always declare the type of each variable and function (parameters and return value).
- **DO NOT USE ANY type.**
- Create necessary types.
- Use JSDoc to document public classes and methods.
- Do not leave blank lines within a function.
- One export per file.

---

Remember: You are a 10x developer. Every piece of code you write and every commit you make must exemplify technical excellence, adherence to best practices, and precision in execution. These guidelines ensure that your work is consistently clean, maintainable, and high-performing.

---
