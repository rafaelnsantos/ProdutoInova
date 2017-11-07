# Produto Inova Contributing Guide

Hi! I’m really excited that you are interested in contributing to Inova. Before submitting your contribution though, please make sure to take a moment and read through the following guidelines.

- [Code of Conduct](https://github.com/rafaelnsantos/ProdutoInova/blob/master/CONTRIBUTING/CODE_OF_CONDUCT.md)
- [Code Style](https://google.github.io/styleguide/javaguide.html)
- [Issue Reporting Guidelines](#issue-reporting-guidelines)
- [Pull Request Guidelines](#pull-request-guidelines)
- [Development Setup](#development-setup)
- [Project Structure](#project-structure)

## Issue Reporting Guidelines

- Always use [https://github.com/rafaelnsantos/ProdutoInova/issues](https://github.com/rafaelnsantos/ProdutoInova/issues) to create new issues.

## Pull Request Guidelines

- The `master` branch is basically just a snapshot of the latest stable release. All development should be done in dedicated branches. **Do not submit PRs against the `master` branch.**

- Checkout a topic branch from the relevant branch, e.g. `dev`, and merge back against that branch.

- It's OK to have multiple small commits as you work on the PR - we will let GitHub automatically squash it before merging.

- Make sure tests passes.

- If adding new feature:
  - Add accompanying test case.
  - Provide convincing reason to add this feature. Ideally you should open a suggestion issue first and have it greenlighted before working on it.

- If fixing a bug:
  - Provide detailed description of the bug in the PR.
  - Add appropriate test coverage if applicable.

## Development Setup

You will need [Java SE Development Kit](http://www.oracle.com/technetwork/java/javase/downloads/index.html) and [PostgreSQL](https://www.postgresql.org/).

Clone the repo.

Import the project in Netbeans.

Run PostgreSQL before running the project.

## Project Structure

- **`doc`**: contains the documentation.

  - `Produto.asta`: contains UML diagrams.

- **`Scripts`**: contains database scripts.

  - `Database.txt`: contains database creation scripts.

- **`Source/src`**: contains the source code.

  - **`main/java/br/data/crud`**: contains code related to the CRUD operations.

  - **`main/java/br/data/entity`**: contains code related to the Models.

  - **`main/resources/META-INF/persistence.xml`**: contains code related to database connection.

  - **`test/java`**: contains all tests.