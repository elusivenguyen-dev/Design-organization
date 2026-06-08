# Contributing Guidelines

Thank you for your interest in contributing! This document provides guidelines and instructions for contributing to this project.

## Getting Started

1. Fork the repository on GitHub
2. Clone your fork locally
3. Create a new branch for your feature or fix
4. Make your changes
5. Push to your fork and submit a Pull Request

## Development Setup

See [docs/DEVELOPMENT.md](docs/DEVELOPMENT.md) for detailed setup instructions.

Quick start:
```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
npm install
npm run dev
```

## How to Contribute

### Reporting Bugs

Before creating a bug report, please check existing issues. When creating a bug report, include:
- Clear description of the bug
- Steps to reproduce
- Expected vs actual behavior
- Screenshots (if applicable)
- Environment details (OS, browser, Node version)

Use the [Bug Report template](.github/ISSUE_TEMPLATE/bug_report.yml).

### Suggesting Features

Feature requests are welcome! Please:
- Check if the feature has already been requested
- Provide clear use case and motivation
- Explain how it benefits the project

Use the [Feature Request template](.github/ISSUE_TEMPLATE/feature_request.yml).

### Pull Requests

1. **Branch naming:**
   - `feature/description` - New features
   - `fix/description` - Bug fixes
   - `docs/description` - Documentation changes
   - `refactor/description` - Code refactoring

2. **Before submitting:**
   - Run `npm run lint` and fix any issues
   - Run `npm run type-check` to ensure TypeScript compiles
   - Run `npm run test` to ensure all tests pass
   - Update documentation if needed

3. **PR description should include:**
   - What changes were made and why
   - Link to related issue(s)
   - Screenshots/GIFs for UI changes
   - Testing instructions

4. **Review process:**
   - All PRs require at least one review
   - Address review comments promptly
   - Maintain a respectful and constructive tone

## Code Standards

### TypeScript
- Use strict TypeScript settings
- Avoid `any` types
- Use meaningful variable names
- Add JSDoc comments for public APIs

### React Components
- Use Server Components by default
- Keep components focused and small
- Use composition over inheritance
- Follow accessibility best practices (WCAG 2.1 AA)

### Styling
- Use Tailwind CSS utility classes
- Follow mobile-first approach
- Use CSS variables for theming
- Ensure responsive design

### Testing
- Write tests for new features
- Maintain minimum 80% coverage
- Test edge cases and error states
- Use descriptive test names

## Commit Messages

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <subject>

<body>

<footer>
```

Types: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `chore`

Example:
```
feat(auth): add OAuth2 login with Google

Implement Google OAuth2 authentication using NextAuth.js.
Includes profile picture sync and account linking.

Closes #123
```

## Documentation

- Update README.md if changing setup instructions
- Update API.md if modifying endpoints
- Update ARCHITECTURE.md if changing system design
- Add JSDoc comments to public functions

## Community

- Be respectful and inclusive
- Provide constructive feedback
- Help others learn and grow
- Follow our [Code of Conduct](CODE_OF_CONDUCT.md)

## Questions?

Feel free to open a [Discussion](https://github.com/your-username/your-repo/discussions) or reach out to maintainers.

## License

By contributing, you agree that your contributions will be licensed under the same license as the project.
