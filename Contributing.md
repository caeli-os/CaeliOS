# Contributing to Caeli OS

Thank you for your interest in contributing to Caeli OS! We welcome contributions of all kinds—from bug reports and documentation improvements to feature implementations and performance optimizations. To make the process smooth and efficient for everyone, please follow these guidelines.

## Table of Contents
1. [Getting Started](#getting-started)
2. [Code of Conduct](#code-of-conduct)
3. [Reporting Issues](#reporting-issues)
4. [Feature Requests](#feature-requests)
5. [Development Workflow](#development-workflow)
   - [Branching Model](#branching-model)
   - [Commit Messages](#commit-messages)
   - [Pull Requests](#pull-requests)
6. [Coding Standards](#coding-standards)
7. [Testing](#testing)
8. [Documentation](#documentation)
9. [Communication](#communication)
10. [License](#license)

---

## Getting Started
1. Fork the repository: click **Fork** in the upper-right corner on GitHub.
2. Clone your fork:
   ```bash
   git clone https://github.com/<your-username>/caeli-os.git
   cd caeli-os
   ```
3. Install prerequisites (Rust, Cargo, target toolchains):
   ```bash
   rustup install stable
   rustup component add rust-src
   ```
4. Build and run tests to verify your setup:
   ```bash
   cargo build
   cargo test
   ```

## Code of Conduct
Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project, you agree to abide by its terms.

## Reporting Issues
If you encounter bugs or unexpected behavior:
1. Check existing issues to avoid duplicates.
2. Open a new issue and include:
   - A clear and descriptive title.
   - Steps to reproduce the problem.
   - Expected vs. actual behavior.
   - Relevant logs, error messages, and environment details.

## Feature Requests
To propose a new feature:
1. Search existing issues to ensure it hasn’t been requested.
2. Open an issue with the `enhancement` label.
3. Provide:
   - A clear description of the feature.
   - Use cases and benefits.
   - (Optional) A rough design or interface sketch.

## Development Workflow
### Branching Model
We use the [GitHub flow](https://guides.github.com/introduction/flow/):
- All work is done on feature branches off `main`.
- After completing work, open a pull request (PR) against `main`.

Branch naming convention:
```
feature/<brief-description>
fix/<brief-description>
docs/<brief-description>
```

### Commit Messages
Follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:
```
<type>(<scope>): <short description>

[optional body]

[optional footer]
```
Types include `feat`, `fix`, `docs`, `style`, `refactor`, `test`, and `chore`.

### Pull Requests
1. Fork and create your branch.
2. Make commits with clear messages.
3. Ensure tests pass and no new warnings are introduced.
4. Push to GitHub and open a PR:
   - Describe the change in detail.
   - Reference relevant issues (e.g., `Closes #123`).
   - Add labels if appropriate.
5. Request reviews from maintainers.

## Coding Standards
- **Rust**: follow [rustfmt](https://github.com/rust-lang/rustfmt) defaults.
- **Documentation**: use [rustdoc](https://doc.rust-lang.org/rustdoc/) for API docs.
- Write clear, concise comments.
- Keep functions focused on a single task.

## Testing
- Add or update unit tests in `tests/` or alongside modules.
- For critical features, include integration tests.
- Run all tests before submitting a PR:
  ```bash
  cargo test
  ```
- Use code coverage tools as needed.

## Documentation
- Update `README.md` for high-level changes.
- Add usage examples in `docs/` for new features.
- Generate API docs:
  ```bash
  cargo doc --open
  ```

## Communication
- Discuss proposals in GitHub issues first.
- For design discussions, use issue threads or create a design doc under `docs/design/`.
- Join our community chat at [Timewalk Discord](https://discord.gg/timewalk) for real-time collaboration.

## License
By contributing, you agree that your contributions will be licensed under the project’s [GPLv3 License](LICENSE.md).

---

Thank you for helping improve Caeli OS! We appreciate your time and expertise.
