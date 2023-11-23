# Git Best Practices Guidelines

This document presents guidelines and best practices for utilizing Git in software development. Adherence to these guidelines helps to maintain an efficient, clean, and effective software development workflow.

## Naming the Branches

A consistent and descriptive branch naming convention enhances collaboration and change tracking. Here are some branch naming guidelines:

- Branch names should convey the changes they introduce.
- If using an issue tracker, include the task ID in the branch name, e.g., `issue-#123`.
- Use lowercase letters and hyphens for separating words to enhance readability.
- Prefix the branch name with a category that represents the type of work, e.g., `feature/`, `bugfix/`, `hotfix/`, `release/`, etc.

Here are some category examples:

- `feature/`: For new features, e.g., `feature/add-user-authentication`.
- `bugfix/` or `fix/`: For bug fixes, e.g., `bugfix/resolve-login-issue`.
- `hotfix/`: For urgent fixes in the production environment, e.g., `hotfix/fix-crashing-bug`.
- `release/`: For new product releases, e.g., `release/v1.0.1`.
- `experiment/`: For new ideas or technologies, e.g., `experiment/try-react-hooks`.
- `refactor/`: For code refactoring, e.g., `refactor/simplify-login-logic`.
- `docs/`: For documentation updates, e.g., `docs/update-readme`.
- `test/`: For test additions or improvements, e.g., `test/add-unit-tests`.
- `chore/`: For routine tasks that do not modify source code, e.g., `chore/update-dependencies`.
- `style/`: For code-style updates or formatting, e.g., `style/implement-prettier`.
- `performance/`: For performance improvements, e.g., `performance/optimize-image-loading`.

## Pull Requests

Include a file named `PULL_REQUEST_TEMPLATE.md` in your project's root directory with the following content to guide pull request creation. This automatically generates a standardized format whenever a pull request is created. Always add a reviewer for a pull request.

```markdown
## Pull Request
### Description
Provide a brief overview of the changes introduced by this PR. Explain the problem being addressed or the feature being implemented.

### Changes Made
Outline the specific changes made in this PR. This can include a bullet list of new features, bug fixes, refactoring, or any other modifications made to the codebase.

### Related Issues
List any related issues or tickets from your project management system (e.g., GitHub issues, JIRA) that are addressed by this PR. Include issue numbers and a brief description.

### Testing Done
Describe the testing performed on the changes in this PR. Include information about the test environment, test cases executed, and any specific testing methodologies followed. If automated tests were added or updated, mention that as well.

### Checklist
- [ ] Manual testing has been performed and passed.
- [ ] Documentation has been updated (if applicable).
- [ ] The branch is up to date with the target branch (e.g., `main` or `master` or `development` or `staging`).

### Additional Notes
Add any additional notes, context, or explanations that can help reviewers.
```

# Commit Messages

Commit messages should follow a standardized format, ensuring clear communication to other developers and automated tools. The structure is as follows:

```
<type>[optional scope]: <description>
```

followed by optional body and footer sections for more detailed information. Here are some examples:

# Changelog

## New Features

- **User Authentication**
  - Description: Add two-factor authentication
  - Commit: `feat(user-auth): add two-factor authentication`

## Bug Fixes

- **Login**
  - Description: Resolve password reset issue
  - Commit: `fix(login): resolve password reset issue`

## Documentation Updates

- **API**
  - Description: Update endpoint descriptions
  - Commit: `docs(api): update endpoint descriptions`

## Code Refactoring

- **User Service**
  - Description: Streamline error handling
  - Commit: `refactor(user-service): streamline error handling`

## Breaking Changes

- **User Profile**
  - Description: Remove support for legacy profile settings
  - Commit: `feat(user-profile)!: remove support for legacy profile settings`
  - Breaking Change Note: `BREAKING CHANGE: The legacy profile settings are no longer supported. Users need to migrate to the new settings.`


# Reviewer Instructions

As a reviewer, you play a vital role in maintaining the quality of our codebase. When reviewing a pull request, consider the following:

1. **Understand the Context**
2. **Validate the Solution**
3. **Check for Tests**
4. **Check for Documentation**
5. **Follow the Commit Guidelines**
6. **Ensure Consistency**

# Reviewer Comments

When reviewing, provide feedback, including:

- Comment on Code Quality
- Comment on Testing
- Comment on Code Style
- Comment on Performance
- Comment on Readability
- Comment on Documentation

Provide clear explanations and suggestions for improvement if there are issues. If the pull request is good, approve it for merging. Remember, code review is a collaborative process, so maintain a positive and constructive tone.

**Author:** Ashish

# Helpful Links

- [Repositories documentation - GitHub Docs](https://docs.github.com/en/repositories)
- [Pull requests documentation - GitHub Docs](https://docs.github.com/en/pull-requests)
- [Authentication documentation - GitHub Docs](https://docs.github.com/en/authentication)
