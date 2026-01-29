# Contributing to go-krb5/krb5

## Current Status

Your fork (`smnsjas/krb5`) is currently **fully synchronized** with the upstream repository (`go-krb5/krb5`). Both repositories are at commit `fdb7902` ("refactor: factorize (#14)"). This means:

- ✅ Your fork has all the latest changes from upstream
- ✅ There are no unique changes in your fork to contribute back
- ✅ You're ready to start making new contributions when needed

## Understanding the Pull Request Process

Since this is your first time contributing to an open-source project, here's a guide to the typical workflow:

### 1. Fork and Clone (Already Done)

You've already forked the repository and cloned it locally. This is your personal copy where you can make changes.

### 2. Keep Your Fork Synchronized

Before making any changes, ensure your fork is up-to-date with upstream:

```bash
# Add upstream remote (if not already added)
git remote add upstream https://github.com/go-krb5/krb5.git

# Fetch latest changes from upstream
git fetch upstream

# Switch to your main branch
git checkout master

# Merge upstream changes
git merge upstream/master

# Push to your fork
git push origin master
```

### 3. Create a Feature Branch

Always create a new branch for your changes:

```bash
# Create and switch to a new branch
git checkout -b feature/my-new-feature

# Or for bug fixes
git checkout -b fix/bug-description
```

### 4. Make Your Changes

- Write clean, well-documented code
- Follow the existing code style
- Add tests for new functionality
- Update documentation as needed

### 5. Test Your Changes

Before submitting, ensure everything works:

```bash
# Run all tests
go test -v ./...

# Run linter (if available)
golangci-lint run

# Build the project
go build ./...
```

### 6. Commit Your Changes

Write clear, descriptive commit messages:

```bash
git add .
git commit -m "feat: add support for XYZ feature"

# Or for bug fixes
git commit -m "fix: resolve issue with ABC"
```

Follow conventional commit format:
- `feat:` for new features
- `fix:` for bug fixes
- `docs:` for documentation changes
- `test:` for adding/modifying tests
- `refactor:` for code refactoring
- `chore:` for maintenance tasks

### 7. Push to Your Fork

```bash
git push origin feature/my-new-feature
```

### 8. Create a Pull Request

1. Go to your fork on GitHub
2. Click "Compare & pull request"
3. Select the upstream repository's `master` branch as the base
4. Provide a clear title and description:
   - What problem does this solve?
   - How does your change work?
   - Any breaking changes?
   - Related issues (if any)

### 9. Respond to Review Feedback

- Maintainers may request changes
- Be open to feedback and suggestions
- Make requested changes in your branch
- Push updates (they'll automatically appear in the PR)

### 10. Wait for Merge

Once approved, maintainers will merge your PR into the upstream repository.

## Best Practices for Contributions

### Before You Start

1. **Check existing issues**: See if someone is already working on it
2. **Open an issue first**: For significant changes, discuss with maintainers
3. **Read project documentation**: Understand coding standards and requirements

### Writing Quality Code

1. **Follow the style guide**: Match existing code patterns
2. **Write tests**: Aim for good test coverage
3. **Document your code**: Add comments for complex logic
4. **Keep commits focused**: One logical change per commit
5. **Avoid breaking changes**: Unless discussed with maintainers

### For This Project Specifically

Based on the repository structure:

- **Language**: Go 1.25+ (check go.mod for current version)
- **Testing**: Use `go test` and ensure all tests pass
- **Code Quality**: The project uses golangci-lint for linting
- **CI/CD**: GitHub Actions runs on PRs (see `.github/workflows/go.yml`)
- **Dependencies**: Use `go mod tidy` to keep dependencies clean

### Common Contribution Types

1. **Bug Fixes**
   - Provide a clear description of the bug
   - Include steps to reproduce
   - Add tests that fail without your fix

2. **New Features**
   - Discuss with maintainers first
   - Ensure it aligns with project goals
   - Include comprehensive tests and documentation

3. **Documentation**
   - Fix typos, improve clarity
   - Add examples
   - Update outdated information

4. **Performance Improvements**
   - Include benchmarks showing improvement
   - Ensure no functionality is broken

## Need Help?

- Check the project's README.md
- Look at recent merged PRs for examples
- Ask questions in GitHub issues
- Be patient and respectful with maintainers

## Important Notes

- The upstream project is maintained by `go-krb5` organization
- Recent activity shows the project is actively maintained
- Major contributors include james-d-elliott and Crowley723
- The project follows semantic versioning
- Breaking changes are documented in BREAKING.md

## Your Next Steps

Since your fork is currently synchronized:

1. **If you have changes to contribute**: Create a feature branch and follow the process above
2. **If you're just learning**: Study the codebase, try fixing a good-first-issue
3. **If you're planning changes**: Open an issue first to discuss with maintainers

Remember: Contributing to open source is a learning process. Don't be afraid to ask questions, and be prepared to iterate on your contributions based on feedback. The community appreciates all contributions, no matter how small!
