# Contributing to AlterLab Python SDK

Thank you for your interest in contributing to the AlterLab Python SDK! This document provides guidelines and instructions for contributing.

## Getting Started

### Prerequisites

- Python 3.8 or higher
- [Poetry](https://python-poetry.org/) for dependency management

### Setup

1. Fork the repository
2. Clone your fork:
   ```bash
   git clone https://github.com/YOUR_USERNAME/python.git
   cd python
   ```

3. Install dependencies:
   ```bash
   poetry install
   ```

4. Run tests to make sure everything works:
   ```bash
   poetry run pytest
   ```

## Development Workflow

### Code Style

We use the following tools to maintain code quality:

- **Black** for code formatting
- **isort** for import sorting
- **Ruff** for linting
- **mypy** for type checking

Run all checks:
```bash
poetry run black alterlab/
poetry run isort alterlab/
poetry run ruff check alterlab/
poetry run mypy alterlab/
```

### Running Tests

```bash
# Run all tests
poetry run pytest

# Run with coverage
poetry run pytest --cov=alterlab --cov-report=html

# Run specific test file
poetry run pytest tests/test_client.py -v
```

### Making Changes

1. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. Make your changes

3. Add tests for any new functionality

4. Ensure all tests pass and code quality checks succeed

5. Commit your changes:
   ```bash
   git commit -m "feat: add your feature description"
   ```

### Commit Messages

We follow [Conventional Commits](https://www.conventionalcommits.org/):

- `feat:` - New features
- `fix:` - Bug fixes
- `docs:` - Documentation changes
- `test:` - Adding or updating tests
- `refactor:` - Code changes that neither fix bugs nor add features
- `chore:` - Maintenance tasks

### Pull Requests

1. Push your branch to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```

2. Open a Pull Request against the `main` branch

3. Fill out the PR template with:
   - Description of changes
   - Related issues (if any)
   - Testing performed

4. Wait for CI checks to pass

5. Request review from maintainers

## Reporting Issues

### Bug Reports

When reporting bugs, please include:

- Python version
- SDK version (`pip show alterlab`)
- Operating system
- Minimal code to reproduce the issue
- Full error traceback

### Feature Requests

For feature requests, please describe:

- The use case
- Expected behavior
- Any alternatives you've considered

## Code of Conduct

- Be respectful and inclusive
- Focus on constructive feedback
- Help maintain a welcoming community

## Questions?

- Open a [GitHub Issue](https://github.com/RapierCraft/AlterLab-SDK/issues)
- Email: dev@alterlab.io
- Documentation: https://alterlab.io/docs

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
