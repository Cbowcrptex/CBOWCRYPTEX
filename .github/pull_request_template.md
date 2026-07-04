name: Pull Request
description: Create a pull request to contribute code

body:
  - type: markdown
    attributes:
      value: |
        Thank you for contributing! Please fill out this form to help us review your PR.

  - type: textarea
    id: description
    attributes:
      label: 📝 Description
      description: Brief description of what this PR does
      placeholder: "What changes are you making?"
    validations:
      required: true

  - type: textarea
    id: motivation
    attributes:
      label: 🎯 Motivation
      description: Why are these changes needed? What problem do they solve?
      placeholder: "Describe the motivation and context"
    validations:
      required: true

  - type: textarea
    id: changes
    attributes:
      label: 🔄 Changes
      description: List the main changes in this PR
      placeholder: |
        - Change 1
        - Change 2
        - Change 3
    validations:
      required: true

  - type: textarea
    id: testing
    attributes:
      label: 🧪 Testing
      description: How should reviewers test this? Include any test commands
      placeholder: |
        1. Run `npm run test`
        2. Check feature works with...
        3. Verify no regressions in...
    validations:
      required: true

  - type: textarea
    id: docs
    attributes:
      label: 📚 Documentation
      description: Were docs updated? Links to doc changes if applicable
      placeholder: "Updated CONTRIBUTING.md, README.md, API docs, etc."

  - type: textarea
    id: breaking
    attributes:
      label: ⚠️ Breaking Changes
      description: Are there any breaking changes? If yes, describe them
      placeholder: "None, or describe breaking changes"

  - type: textarea
    id: issues
    attributes:
      label: 🔗 Related Issues
      description: Link to related issues (e.g., Fixes #123, Related to #456)
      placeholder: "Fixes #123"

  - type: dropdown
    id: type
    attributes:
      label: 📌 PR Type
      options:
        - Feature
        - Bug Fix
        - Documentation
        - Refactoring
        - Performance
        - Tests
        - Other
    validations:
      required: true

  - type: checkboxes
    id: checklist
    attributes:
      label: ✅ Checklist
      description: Please verify all these items before submitting
      options:
        - label: Tests pass locally (`npm run test`)
          required: true
        - label: Code follows style guide (`npm run lint`)
          required: true
        - label: Code is formatted (`npm run format`)
          required: true
        - label: Commits use conventional format
          required: true
        - label: No merge conflicts
          required: true
        - label: Documentation updated (if needed)
          required: false
        - label: No new warnings generated
          required: false

  - type: markdown
    attributes:
      value: |
        Thank you for your contribution! We'll review this as soon as possible.
