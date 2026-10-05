# AGENTS.md

Context file for AI agents working on meteor.

**Dual Format**: This file combines Category A (Operations Manual) and Category B (Context Guide) for comprehensive agent guidance.

## Project Overview

meteor is a Javascript project using npm/Node.js.

**Key Info:**
- **Primary Language:** Javascript
- **Build System:** npm/Node.js
- **Test Framework:** Mocha
- **Total Files:** 4399
- **Test Files:** 1729
- **AI Readiness Score:** 88/100 (AI-Native-Plus)

---

## 🚨 AI Policy & Operations

Extracted from CONTRIBUTING.md - operational constraints and procedures.

### AI Policy

- We are excited to have your help building Meteor &mdash; both the platform and the community behind it. Please read the project overview and guidelines for contributing bug reports and new code, or it might be hard for the community to help you with your issue or pull request.
- Before we jump into detailed guidelines for opening and triaging issues and submitting pull requests, here is some information about how our project is structured and resources you should refer to as you start contributing.
- If you'd like to contribute to Meteor's documentation, head over to https://docs.meteor.com/community/contributing.html for guidelines.
- standards for API design, for the names of symbols, for documentation,
- developer.  That can be a difficult standard to reach, because we're

### Key Requirements

- There are many ways to contribute to the Meteor Project. Here’s a list of technical contributions with increasing levels of involvement and required knowledge of Meteor’s code and operations.
- Any issue that does not have the `ready` label still requires discussion on implementation details, but input and positive commentary are welcome! Any pull request opened on an issue that is not `confirmed` is still welcome. However, the pull request is more likely to be sent back for reworking than a `ready` issue.
- need to do.
- request. In addition to the core code change, attention needs to be paid to
- Above all, we are concerned with two design requirements when evaluating

### Development Procedures

- To quickly check out a PR branch from a fork for local testing, see the [Testing a fork branch](DEVELOPMENT.md#testing-a-fork-branch) section in `DEVELOPMENT.md`, or run:
- npm run checkout:pr -- https://github.com/meteor/meteor/pull/<PR-number>
- The TSC is the governing body responsible for major, long-term decisions about Meteor — architectural direction, breaking changes, and project-wide policies. TSC members hold commit access to meteor/meteor, and publishing official Meteor releases is their exclusive domain. The TSC is composed of Meteor Software employees and is **not** open to community nomination. See [GOVERNANCE.md](GOVERNANCE.md) for details.
- Right now, the best place to track the work being done on Meteor is to take a look at the latest release milestone [here](https://github.com/meteor/meteor/milestones).  Also, the [Meteor Roadmap](https://docs.meteor.com/about/roadmap.html) contains high-level information on the current priorities of the project.
- should include a link to a repository with a reproduction. By making it as easy as possible



## 🏗️ Architecture & Context Guide

This section provides architectural context and agent-understanding for the codebase.

### Prerequisites

- **Javascript:** 16+ (or applicable language version)
- **Package Manager:** npm or yarn
- **Test Runner:** Mocha



### Project Structure

```
meteor/
├── package.json
├── package.json
├── package.json
├── src/                  # Source code
├── tests/                # Test suite (1729 files)
└── README.md             # Project documentation
```

### Architecture Overview

#### Key Components
- **Main Entry:** index.js, index.js, main.js, main.js, main.js
- **Test Suite:** 1729 test files
- **Build Configuration:** package.json, package.json, package.json

#### Design Principles

1. **Modularity** - Code organized by functionality with clear separation of concerns
2. **Testability** - Comprehensive test coverage across critical paths
3. **Clarity** - Explicit naming and structure for AI agent understanding
4. **Consistency** - Uniform patterns and conventions throughout codebase
5. **Maintainability** - Well-documented code with clear intent

### Directory Map

| Directory | Purpose |
|-----------|----------|
| `docs/` | Documentation |
| `scripts/` | Build and utility scripts |


### Development Workflow

#### Initial Setup

```bash
git clone https://github.com/jaykrishna316/meteor.git
cd meteor
npm install
# or
yarn install
```

#### Development Commands

**Running Tests:**
```bash
npm test                  # Run all tests
npm run test -- --watch   # Watch mode
npm run lint              # Lint code
```

#### Code Quality
```bash
npm run format            # Format code (prettier)
npm run lint -- --fix     # Auto-fix lint issues
```

### Code Style & Conventions

- **Naming:** Use Javascript conventions (camelCase for functions, PascalCase for classes)
- **Type Hints:** Yes (strongly encouraged)
- **Error Handling:** Yes - handle errors at boundaries; let exceptions propagate when another layer owns recovery
- **Logging:** Yes
- **Testing:** Yes - write tests alongside code changes

### Testing Strategy

**Framework:** Mocha
**Test Files:** 1729 found

Before committing:
1. Run the full test suite: `npm test` or `yarn test`
2. Run linter: `npm run lint` or `yarn lint`
3. Format code: `npm run format` or `yarn format`
4. Type check (if TypeScript): `npm run typecheck`

### Writing Documentation

When updating docs:
1. Always include explanatory text before code snippets
2. Describe *why* and *what* before showing *how*
3. Keep sections focused on a single concept
4. Use clear, concrete examples

## Known Gotchas & Warnings

- the server (not always workable; we don't have fibers on the client or a DOM on the server).  We
- docs don't force new users to understand advanced concepts before they

### Contributing Guidelines

This project has a detailed contribution guide at **`CONTRIBUTING.md`**.

**Key Requirements:**
- Review the contribution guide for all requirements
- Follow established patterns in the codebase
- Ensure alignment with project's contribution policies

### Common Patterns

When contributing to this project:
1. Read existing code in the area you're modifying
2. Follow the established patterns and style
3. Write tests for new functionality
4. Use clear, descriptive variable and function names
5. Add docstrings for public APIs
6. Update tests when changing behavior

### What We Value

✅ Well-tested code with clear intent
✅ Consistent code style and naming conventions
✅ Code that is easy for AI agents to understand
✅ Clear, descriptive commit messages
✅ Modular, reusable components
✅ Comprehensive documentation

### What We Avoid

❌ Large functions doing multiple things
❌ Commented-out dead code
❌ Inconsistent naming or patterns
❌ Unclear error messages
❌ Unexplained magic numbers or strings
❌ Skipped tests or test TODOs

### AI Readiness Dimensions (Scoring)

This project is evaluated across 8 dimensions:

1. **Architecture** (20/100) - Code organization and modularity
2. **Testing** (15/100) - Test coverage and quality
3. **Dependencies** (12/100) - Dependency management
4. **Conventions** (8/100) - Consistent patterns
5. **Entry Points** (10/100) - Clear main/start locations
6. **Security** (5/100) - Input validation and error handling
7. **Build** (10/100) - Clear build/setup instructions
8. **Documentation** (8/100) - Code and project documentation

### Next Steps

Before making changes:
1. Read relevant source files to understand the existing code
2. Look at existing tests for similar functionality
3. Follow the patterns you see in the codebase
4. Write tests for your changes
5. Run `npm test` to verify nothing breaks
6. Run linter: `npm run lint`
7. Format your code: `npm run format`

---

*Generated by Braxis - keeping AI agents in sync with your code*

