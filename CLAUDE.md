# Data Universe Development Guide

## Build & Installation
- Initial setup: `pip install -e .`
- Install requirements: `pip install -r requirements.txt`

## Testing
- Run all tests: `python tests/test_all.py`
- Run single test: `python -m unittest tests/path/to/test_file.py`
- Run specific test class: `python -m unittest tests.path.to.test_file.TestClassName`
- Run specific test method: `python -m unittest tests.path.to.test_file.TestClassName.test_method_name`

## Code Style Guidelines
- **Naming**: Use snake_case for variables/functions, PascalCase for classes, UPPER_CASE for constants
- **Imports**: Standard library → Third-party libraries → Project modules
- **Type Hints**: Required for function parameters and return values
- **Docstrings**: Triple-quoted strings with parameter descriptions
- **Error Handling**: Catch specific exceptions, use bt.logging for errors
- **Patterns**: Use Pydantic models for validation, async/await for async operations
- **Organization**: Keep related functionality in appropriate modules

## Common Libraries
- bittensor: For neuron framework, logging, and subtensor interaction
- pydantic: For data validation and typing
- loguru: For enhanced logging