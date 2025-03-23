# Project Rules: Nuxt 3 + TypeScript + NestJS + Drizzle ORM

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
- Avoid extraneous commentary or summaries that are not directly related to the change.
- **Examples**:
- `feat(api): implement new authentication endpoint with NestJS`
- `fix(service): resolve issue with data transformation in Drizzle ORM query`
- `refactor(controllers): streamline request handling in NestJS endpoints`

---

## 2. Code Quality and Development Principles

### Clean Code & Best Practices
- **Simplicity**:
- Write simple, clear, and straightforward code. Avoid unnecessary complexity.
- Every line of code should add clear value; remember that extra code increases technical debt.
- **Readability & Maintainability**:
- Use descriptive and explicit variable names (e.g., `isLoading`, `hasError`).
- Organize files to clearly separate exported components, subcomponents, helpers, static content, and types.
- Preserve the existing formatting of imports and code structure—do not alter formatting unless essential for new functionality.
- **DRY (Don't Repeat Yourself)**:
- Eliminate code duplication by modularizing common logic into reusable functions or modules.
- **Functional Paradigm**:
- Prefer functional programming patterns when possible—use pure functions, immutability, and avoid side effects.
- While NestJS is class-based, ensure that business logic within services and controllers remains concise and testable.
- **SOLID Principles**:
- **Single Responsibility**: Each function or module should handle one distinct task.
- **Open/Closed**: Write code that is extendable without modifying existing functionality.
- **Liskov Substitution**: Ensure that modules can be replaced with abstractions without breaking the system.
- **Interface Segregation**: Create smaller, focused interfaces for specific purposes.
- **Dependency Inversion**: Depend on abstractions rather than concrete implementations.
- **KISS (Keep It Simple, Stupid)**:
- Favor simple and direct solutions over unnecessarily clever or convoluted implementations.

---

## 3. Response and Code Change Guidelines

### Expected Behavior from Cursor Responses
- **Precision and Technicality**:
- Responses must be precise and technical, providing only the necessary changes along with detailed code examples in TypeScript.
- Deliver all modifications as a single cohesive block—avoid splitting changes over multiple steps.
- **Code Formatting & Structure**:
- **Do Not** modify existing code, comments, or formatting unless it is critical for implementing new functionality.
- Preserve the original formatting of imports, comments, and code sections.
- **Adherence to Guidelines**:
- Every response must follow the established Git commit conventions and clean code principles.
- Ensure the solution is modular, DRY, and leverages a functional programming approach where applicable.
- **No Extraneous Information**:
- Do not include unnecessary apologies, confirmations, or summary remarks.
- Avoid suggesting changes related to whitespace or formatting unless absolutely necessary.
- **Explicit Variable Naming**:
- Use clear and descriptive variable names that accurately convey their purpose.
- **Performance and Security**:
- Optimize code for performance using efficient data structures and algorithms.
- Always consider security implications, particularly when handling user input and data transactions.
- **Testing and Error Handling**:
- Include unit tests for new or modified code when applicable.
- Implement robust error handling and logging, especially in data access layers.

---

## 4. Specific Guidelines for Nuxt 3 + TypeScript + NestJS + Drizzle ORM Projects

### Technology-Specific Instructions
- **Nuxt 3 & TypeScript**:
- Utilize Nuxt 3’s file-based routing and server-side rendering features.
- Leverage TypeScript for static type-checking, ensuring all types and interfaces are declared and used consistently.
- **NestJS Integration**:
- Use NestJS to structure the backend, organizing code into modules, controllers, and services.
- Keep controllers thin: delegate business logic to services.
- Ensure middleware, guards, and interceptors are used appropriately for security and performance.
- **Drizzle ORM**:
- Integrate Drizzle ORM for database operations.
- Write clear and type-safe database queries using Drizzle ORM’s syntax.
- Abstract database operations in dedicated service layers to maintain separation of concerns.
- Ensure that all database interactions are properly validated and error-handled.
- **Folder Structure and Naming**:
- Use lowercase with dashes for directory names (e.g., `components/auth-wizard`).
- Favor named exports for components, controllers, services, and modules.
- **Code Examples**:
- All code examples must be concise, functional TypeScript code.
- Follow patterns of modularization and reusability using helper functions and composable services.
- Ensure that NestJS-specific modules and Drizzle ORM interactions are cleanly separated from UI logic.

---

## 5. TypeScript General Guidelines (For All Projects)

### Basic Principles
- Use English for all code and documentation.
- Always declare the type of each variable and function (parameters and return value).
- **DO NOT USE ANY type.**
- Create necessary types.
- Use JSDoc to document public classes and methods.
- Don't leave blank lines within a function.
- One export per file.

### Nomenclature
- Use PascalCase for classes.
- Use camelCase for variables, functions, and methods.
- Use kebab-case for file and directory names.
- Use UPPERCASE for environment variables.
- Avoid magic numbers and define constants.
- Start each function with a verb.
- Use verbs for boolean variables. Example: isLoading, hasError, canDelete, etc.
- Use complete words instead of abbreviations and correct spelling.
- Except for standard abbreviations like API, URL, etc.
- Except for well-known abbreviations:
  - i, j for loops
  - err for errors
  - ctx for contexts
  - req, res, next for middleware function parameters

### Functions
- Write short functions with a single purpose. Less than 20 instructions.
- Name functions with a verb and something else.
- If a function returns a boolean, use isX, hasX, canX, etc.
- If it doesn't return anything, use executeX or saveX, etc.
- Avoid nesting blocks by:
- Using early checks and returns.
- Extracting logic to utility functions.
- Use higher-order functions (map, filter, reduce, etc.) to avoid deep nesting.
- Use arrow functions for simple functions (less than 3 instructions).
- Use named functions for non-simple functions.
- Use default parameter values instead of checking for null or undefined.
- Reduce function parameters by:
- Using an object to pass multiple parameters.
- Using an object to return results.
- Declaring necessary types for input arguments and output.
- Use a single level of abstraction.

### Data
- Encapsulate data in composite types rather than using primitive types excessively.
- Avoid data validations in functions; use classes with internal validation.
- Prefer immutability for data.
- Use `readonly` for data that doesn't change.
- Use `as const` for literals that don't change.

### Classes
- Follow SOLID principles.
- Prefer composition over inheritance.
- Declare interfaces to define contracts.
- Write small classes with a single purpose:
- Less than 200 instructions.
- Less than 10 public methods.
- Less than 10 properties.

### Exceptions
- Use exceptions to handle unexpected errors.
- Catch exceptions to:
- Fix an expected problem.
- Add context.
- Otherwise, use a global handler.

### Testing
- Follow the Arrange-Act-Assert convention for tests.
- Name test variables clearly.
- Use the convention: inputX, mockX, actualX, expectedX, etc.
- Write unit tests for each public function.
- Use test doubles to simulate dependencies, except for inexpensive third-party dependencies.
- Write acceptance tests for each module.
- Follow the Given-When-Then convention.

---

## 6. Specific Guidelines for NestJS

### Basic Principles
- Use modular architecture.
- Encapsulate the API in modules:
- One module per main domain/route.
- One controller per route.
- Additional controllers for secondary routes.
- A models folder for data types.
- DTOs validated with `class-validator` for inputs.
- Declare simple types for outputs.
- A services module containing business logic and persistence.
- Entities with MikroORM for data persistence.
- One service per entity.
- Create a core module for NestJS artifacts:
- Global filters for exception handling.
- Global middlewares for request management.
- Guards for permission management.
- Interceptors for request management.
- Create a shared module for services shared across modules:
- Utilities.
- Shared business logic.

### Testing in NestJS
- Use the standard Jest framework for testing.
- Write tests for each controller and service.
- Write end-to-end tests for each API module.
- Add an admin/test method to each controller as a smoke test.

---

Remember: You are a 10x developer. Every piece of code you write and every commit you make must exemplify technical excellence, adherence to best practices, and precision in execution. These guidelines ensure that your work is consistently clean, maintainable, and high-performing.

---