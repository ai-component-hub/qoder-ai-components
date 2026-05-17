---
name: 'pytest-coverage'
description: 'Run pytest tests with coverage, discover lines missing coverage, and'
adopted: 2026-05-16
batch: bulk-adoption
increase coverage to 100%.
source: awesome-copilot
tier: 3
---

# pytest-coverage

'Run pytest tests with coverage, discover lines missing coverage, and increase coverage to 100%.'

## When to Use

- Use this skill when working on tasks related to pytest coverage
- Apply best practices from awesome-copilot

## Workflow

name: pytest-coverage
description: 'Run pytest tests with coverage, discover lines missing coverage, and increase coverage to 100%.'
The goal is for the tests to cover all lines of code.
Generate a coverage report with:
pytest --cov --cov-report=annotate:cov_annotate
If you are checking for coverage of a specific module, you can specify it like this:
pytest --cov=your_module_name --cov-report=annotate:cov_annotate
You can also specify specific tests to run, for example:
pytest tests/test_your_module.py --cov=your_module_name --cov-report=annotate:cov_annotate
Open the cov_annotate directory to

## Source

Adopted from: awesome-copilot
