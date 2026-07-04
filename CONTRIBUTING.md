# Contributing to Cbowcrptex

Thank you for your interest in contributing! We're excited to have you join our community of builders.

---

## 📋 Code of Conduct

We are committed to providing a welcoming and inspiring community for all. Please be respectful, inclusive, and professional in all interactions.

**TL;DR:** Be nice, be respectful, no harassment. More details in our [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md).

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- Git
- Basic understanding of TypeScript/JavaScript
- Familiarity with Web3 concepts (for blockchain features)

### Local Development Setup

```bash
# 1. Fork the repository
# (Click "Fork" on GitHub)

# 2. Clone your fork
git clone https://github.com/YOUR_USERNAME/CBOWCRYPTEX.git
cd CBOWCRYPTEX

# 3. Add upstream remote
git remote add upstream https://github.com/Cbowcrptex/CBOWCRYPTEX.git

# 4. Install dependencies
npm install

# 5. Create a feature branch
git checkout -b feature/your-feature-name

# 6. Set up environment variables
cp .env.example .env.local
# Fill in required API keys and config

# 7. Start development server
npm run dev
```

---

## 🔄 Development Workflow

### 1. **Create an Issue** (for significant changes)
Before starting work on a major feature or bug fix, please create an issue to discuss:
- The problem you're solving
- Your proposed solution
- Any potential impacts
- Questions or concerns

**Issue format:**
```markdown
## What's the issue?
[Describe the problem]

## Proposed solution
[How you plan to fix it]

## Additional context
[Any relevant information]
```

### 2. **Create a Feature Branch**
```bash
git checkout -b feature/your-feature-name
# or for bug fixes
git checkout -b fix/issue-number-short-description
```

**Branch naming conventions:**
- `feature/` - New features
- `fix/` - Bug fixes
- `docs/` - Documentation updates
- `refactor/` - Code refactoring
- `test/` - Test additions/improvements
- `chore/` - Dependencies, config, etc.

### 3. **Make Your Changes**

#### Code Style Guide

**TypeScript/JavaScript:**
```typescript
// Use const by default, let when needed
const myVar = 42;

// Use type annotations
const add = (a: number, b: number): number => a + b;

// Use meaningful names
const getUserById = async (id: string): Promise<User> => {
  // Implementation
};

// Comment complex logic
// Calculate compound interest with daily compounding
const interest = principal * Math.pow(1 + rate / 365, days);
```

**Formatting:**
- 2 spaces for indentation
- Semicolons required
- Max line length: 100 characters (except URLs)
- Use ESLint and Prettier (run `npm run lint` and `npm run format`)

**Commits:**
```bash
# Use conventional commits
git commit -m "feat: add user authentication system"
git commit -m "fix: resolve memory leak in agent loop"
git commit -m "docs: update installation guide"
git commit -m "refactor: simplify token validation"
git commit -m "test: add tests for DeFi calculations"
```

**Conventional commit types:**
- `feat:` - New feature
- `fix:` - Bug fix
- `docs:` - Documentation
- `style:` - Code style (formatting, missing semicolons, etc.)
- `refactor:` - Code refactoring
- `perf:` - Performance improvements
- `test:` - Tests
- `chore:` - Build, dependencies, etc.

### 4. **Write & Run Tests**

```bash
# Run all tests
npm run test

# Run tests in watch mode
npm run test:watch

# Run tests with coverage
npm run test:coverage

# Lint code
npm run lint

# Format code
npm run format
```

**Test requirements:**
- New features should have tests
- Bug fixes should include regression tests
- Aim for >80% code coverage
- Tests should be clear and focused

### 5. **Keep Your Branch Updated**

```bash
# Fetch latest changes from upstream
git fetch upstream

# Rebase your branch
git rebase upstream/main

# If you have conflicts, resolve them and continue
git add .
git rebase --continue
```

### 6. **Submit a Pull Request**

#### Before submitting:
- [ ] Tests pass locally (`npm run test`)
- [ ] Linter passes (`npm run lint`)
- [ ] Code is formatted (`npm run format`)
- [ ] Commits use conventional format
- [ ] No merge conflicts

#### PR Title Format:
Use conventional commits format:
```
type(scope): brief description

Examples:
feat(trading): add market order execution
fix(agent): resolve race condition in loop
docs: update setup instructions
```

#### PR Description Template:
```markdown
## 📝 Description
Brief description of what this PR does

## 🎯 Motivation
Why are these changes needed? What problem do they solve?

## 🔄 Changes
- Change 1
- Change 2
- Change 3

## 🧪 Testing
How to test these changes? Include steps if applicable.

## 📋 Checklist
- [ ] Tests added/updated
- [ ] Documentation updated
- [ ] Code follows style guide
- [ ] No breaking changes

## 🔗 Related Issues
Fixes #123 or Related to #456
```

---

## 📝 Documentation

### When to update docs:
- New features
- API changes
- Bug fixes affecting usage
- Configuration changes

### Documentation types:
1. **Code comments** - Complex logic, "why" not "what"
2. **README files** - Overview, quick start, links
3. **CONTRIBUTING.md** - Setup, workflow, guidelines
4. **API docs** - Function signatures, parameters, examples
5. **Guides** - Step-by-step tutorials

### Doc style:
- Clear, concise language
- Examples for complex concepts
- Keep it up-to-date
- Use code syntax highlighting

---

## 🐛 Bug Reports

If you find a bug:

### Before opening an issue:
1. Check if the issue already exists
2. Try to reproduce with latest code
3. Gather relevant information

### Issue template:
```markdown
## Bug Description
Clear and concise description of the bug

## Steps to Reproduce
1. Do this
2. Then this
3. Then observe this

## Expected Behavior
What should happen

## Actual Behavior
What actually happens

## Environment
- OS: [e.g. macOS, Windows, Linux]
- Node version: [e.g. 18.0.0]
- Version: [e.g. 1.0.0]

## Logs/Screenshots
Include relevant error messages or screenshots

## Additional Context
Any other relevant information
```

---

## ✨ Feature Requests

Have an idea? Share it!

### Feature request template:
```markdown
## Feature Description
Clear description of what you want to add

## Motivation
Why would this be useful? What problems does it solve?

## Proposed Solution
How should this feature work?

## Alternatives
Have you considered other approaches?

## Additional Context
Links, examples, or other relevant info
```

---

## 🚢 Release Process

### Version numbering (Semantic Versioning):
- **MAJOR.MINOR.PATCH** (e.g., 1.2.3)
- MAJOR: Breaking changes
- MINOR: New features (backward compatible)
- PATCH: Bug fixes

### Release checklist:
- [ ] Tests passing
- [ ] Docs updated
- [ ] Changelog updated
- [ ] Version bumped
- [ ] Tag created
- [ ] Release notes published

---

## 💬 Getting Help

### Resources:
- **Documentation** - Check [docs/](./docs/) folder
- **GitHub Discussions** - Ask questions [here](../../discussions)
- **Issues** - Search existing issues
- **Community** - Join our Telegram/X

### Asking for help:
1. Search for existing answers
2. Provide clear, detailed information
3. Be specific about what you're trying to do
4. Include error messages and reproduction steps

---

## 🏆 Recognition

Contributors are recognized in:
- [CONTRIBUTORS.md](./CONTRIBUTORS.md)
- GitHub contributors page
- Release notes (for significant contributions)

---

## 📋 Review Process

When you submit a PR:

1. **Automated checks** - Tests, linting, format
2. **Maintainer review** - Code quality, design, fit
3. **Community feedback** - Questions, suggestions
4. **Revisions** - Address feedback if needed
5. **Merge** - Once approved

**Review time:** Usually 2-7 days depending on complexity

### What we look for:
- ✅ Solves the stated problem
- ✅ Follows code style
- ✅ Includes tests
- ✅ Clear, descriptive commits
- ✅ Updated documentation
- ✅ No breaking changes (unless necessary)

---

## ⚖️ License

By contributing, you agree your code is licensed under the MIT License. See [LICENSE](./LICENSE).

---

## 🙏 Thank You!

We appreciate your contribution to making Cbowcrptex better. You're part of building the future of Web3! 🚀

---

**Questions?** Open an issue or reach out in [Discussions](../../discussions)
