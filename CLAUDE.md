# CLAUDE.md - AI Assistant Guidelines

> This document provides guidance for AI assistants (like Claude) working with this codebase.

## Repository Overview

**Repository:** seahuijang/seahuijang
**Status:** New repository (initialized)
**Last Updated:** 2026-02-03

This is a newly initialized repository. As the project develops, this document should be updated to reflect the actual codebase structure, conventions, and workflows.

---

## Project Structure

```
seahuijang/
├── CLAUDE.md           # AI assistant guidelines (this file)
└── (project files to be added)
```

### Planned/Recommended Structure

When adding code to this repository, consider organizing it as follows:

```
seahuijang/
├── CLAUDE.md           # AI assistant guidelines
├── README.md           # Project documentation
├── LICENSE             # License file
├── .gitignore          # Git ignore patterns
│
├── src/                # Source code
│   ├── main/           # Main application code
│   └── lib/            # Shared libraries/utilities
│
├── tests/              # Test files
│   ├── unit/           # Unit tests
│   └── integration/    # Integration tests
│
├── docs/               # Documentation
│   ├── api/            # API documentation
│   └── guides/         # User guides
│
├── scripts/            # Build/utility scripts
├── config/             # Configuration files
└── .github/            # GitHub workflows and templates
    └── workflows/      # CI/CD workflows
```

---

## Development Workflow

### Getting Started

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd seahuijang
   ```

2. Set up your development environment (instructions to be added based on chosen tech stack)

3. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```

### Branch Naming Conventions

- `main` or `master` - Production-ready code
- `develop` - Development branch (if using git-flow)
- `feature/*` - New features
- `bugfix/*` - Bug fixes
- `hotfix/*` - Urgent production fixes
- `release/*` - Release preparation
- `claude/*` - AI assistant working branches

### Commit Message Format

Follow conventional commits format:

```
<type>(<scope>): <description>

[optional body]

[optional footer]
```

**Types:**
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code refactoring
- `test`: Adding or updating tests
- `chore`: Maintenance tasks
- `perf`: Performance improvements
- `ci`: CI/CD changes

**Examples:**
```
feat(auth): add user authentication system
fix(api): resolve null pointer exception in user endpoint
docs(readme): update installation instructions
```

---

## Code Conventions

### General Guidelines

1. **Keep it simple** - Write clear, readable code
2. **DRY (Don't Repeat Yourself)** - Extract common logic into reusable functions
3. **Single Responsibility** - Each function/class should do one thing well
4. **Meaningful names** - Use descriptive variable and function names
5. **Comment wisely** - Explain "why", not "what"

### File Naming

- Use lowercase with hyphens for files: `user-service.js`, `api-client.py`
- Use PascalCase for class files if language convention requires: `UserService.java`
- Test files should mirror source files: `user-service.test.js`

### Code Style

(To be updated based on chosen tech stack and linting configuration)

- Use consistent indentation (2 or 4 spaces, or tabs - be consistent)
- Maximum line length: 80-120 characters
- Use meaningful whitespace to improve readability
- Group related imports together

---

## Testing

### Test Structure

(To be configured based on chosen testing framework)

```
tests/
├── unit/               # Fast, isolated unit tests
├── integration/        # Tests that verify component interaction
└── e2e/               # End-to-end tests (if applicable)
```

### Running Tests

```bash
# Commands to be added based on tech stack
# Example patterns:
# npm test              # Node.js
# pytest                # Python
# cargo test            # Rust
# go test ./...         # Go
```

### Test Conventions

- Each test should be independent
- Use descriptive test names that explain what is being tested
- Follow the Arrange-Act-Assert (AAA) pattern
- Mock external dependencies in unit tests

---

## Build and Deployment

### Build Commands

(To be configured based on build system)

```bash
# Build commands to be added
# Examples:
# npm run build
# make build
# cargo build --release
```

### Environment Configuration

- Use environment variables for configuration
- Never commit secrets or credentials
- Use `.env.example` to document required environment variables

### Deployment

(Deployment process to be documented)

---

## AI Assistant Guidelines

### When Working on This Codebase

1. **Always read before modifying** - Understand existing code before making changes
2. **Make minimal changes** - Only modify what's necessary for the task
3. **Follow existing patterns** - Match the style and conventions already in use
4. **Run tests** - Verify changes don't break existing functionality
5. **Update documentation** - Keep docs in sync with code changes

### Security Considerations

- Never commit sensitive data (API keys, passwords, tokens)
- Validate all user inputs
- Use parameterized queries for database operations
- Follow OWASP guidelines for web applications
- Review dependencies for known vulnerabilities

### Common Tasks

#### Adding a New Feature

1. Create a feature branch
2. Implement the feature following code conventions
3. Add tests for new functionality
4. Update relevant documentation
5. Create a pull request with clear description

#### Fixing a Bug

1. Create a bugfix branch
2. Write a failing test that reproduces the bug
3. Fix the bug
4. Verify the test passes
5. Check for similar issues elsewhere
6. Create a pull request

#### Code Review Checklist

- [ ] Code follows project conventions
- [ ] Tests are included and passing
- [ ] Documentation is updated
- [ ] No security vulnerabilities introduced
- [ ] Changes are minimal and focused
- [ ] Commit messages are clear and descriptive

---

## Dependencies

### Production Dependencies

(To be documented as dependencies are added)

### Development Dependencies

(To be documented as dependencies are added)

---

## Troubleshooting

### Common Issues

(To be documented as the project develops)

### Getting Help

- Check existing issues in the repository
- Review documentation in `/docs`
- Create a new issue with detailed description

---

## Updating This Document

This CLAUDE.md should be updated whenever:

- New technologies or frameworks are added
- Development workflows change
- New conventions are established
- Build or deployment processes change
- Important project context is added

Keep this document accurate and concise to help AI assistants work effectively with the codebase.

---

## Quick Reference

| Task | Command |
|------|---------|
| Install dependencies | (to be added) |
| Run development server | (to be added) |
| Run tests | (to be added) |
| Build for production | (to be added) |
| Lint code | (to be added) |
| Format code | (to be added) |

---

*This document was generated for an empty repository and should be updated as the project develops.*
