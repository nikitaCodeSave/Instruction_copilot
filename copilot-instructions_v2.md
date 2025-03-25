# Must comply with the instructions outlined here as well as your project's dedicated project assignment document.

## 1. Code Style and Conventions

- **PEP8 Compliance**: Always adhere to PEP8 formatting and style guidelines. Ensure code is neatly organized and maintains readability.
- **Conciseness**: Strive for concise code that is free of unnecessary complexity or repetition. Whenever possible, remove redundant code blocks.
- **Maintainability**: Organize logic in a way that is straightforward for other developers to read, understand, and maintain.

## 2. Dependencies

- **Use Existing Stack**: Prioritize libraries already declared in the project’s `requirements.txt`. Avoid introducing new dependencies unless strictly necessary for project requirements.
- **Updating and Adding Libraries**: 
  - Update existing libraries only if outdated functionality blocks development or if critical security patches are required.
  - Add new libraries only if they provide essential capabilities not available in the existing stack.
  - Always record any updates or additions in `requirements.txt`, respecting version constraints as needed.

## 3. Code Modification and Error Fixes

- **Targeted Fixes**: When correcting errors, limit your changes strictly to the relevant code segments. Refrain from rewriting entire modules or introducing new designs unless explicitly instructed.
- **Code Preservation**: Preserve the original design and business logic unless the project owner explicitly asks for significant refactoring or a complete rewrite.

## 4. Project Architecture

- **Existing Structure**: Adhere to the current project structure, respecting folder organization and naming conventions. Avoid reorganizing or renaming folders/modules without approval.
- **Logical Grouping**: Ensure any new modules or files align logically with the established structure, e.g., placing them in appropriate folders such as `src/`, `utils/`, or `services/`.

## 5. Testing

- **Dedicated Test Folder**: All test files must reside in a dedicated folder (e.g., `tests/`). Follow a consistent naming pattern for test scripts, such as `test_<module_name>.py`.
- **Coverage and Maintenance**: When adding new features, ensure corresponding tests are implemented. Avoid introducing features without proper testing.

## 6. Documentation and Comments

- **Docstrings**:
  - Use Python docstrings (`""" ... """`) for modules, classes, and functions.
  - Provide clear, descriptive explanations regarding functionality, input parameters, return values, and potential exceptions.
- **README File**:
  - Update `README.md` to reflect any new functionality, setup instructions, or relevant changes.

## 7. Logging and Exception Handling

- **Use Standard Libraries**: Utilize Python’s built-in libraries (e.g., `logging`) for error handling and logging. 
- **Minimal Overhead**: Unless explicitly required, avoid extra logging frameworks or third-party packages that may introduce unnecessary dependencies.

## 8. Performance and Optimization

- **Readability First**: Write code that is both clear and adequately optimized. Never sacrifice clarity for micro-optimizations unless performance metrics demand it.
- **Data Structures**: Use appropriate data structures and algorithms. Prioritize maintainability and clarity without ignoring critical performance considerations.

## 9. Reference the Project Assignment Document

- **Contextual Awareness**: Copilot should consult the project assignment document for any domain-specific instructions on architecture, coding patterns, or library usage.
- **Alignment**: All code contributions must remain consistent with the guidelines and objectives specified in the project assignment document.

---

**Usage Reminder**: These guidelines ensure consistency, maintainability, and high-quality code output from Copilot. They also uphold essential industry standards to pass code reviews at leading tech organizations like Google.

