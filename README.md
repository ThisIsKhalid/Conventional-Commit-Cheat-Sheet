# Conventional Commit Cheat Sheet

A comprehensive guide to mastering the [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0/) standard for versioning in your projects.

---
## 🚀 Why Use Conventional Commits?

Conventional Commits provide a standardized way to write commit messages, enabling:

- **Better Collaboration**: Clear commit messages make teamwork more effective.
- **Improved Project Management**: Easily track changes, bugs, and features.
- **Automated Versioning**: Tools like semantic-release can automate versioning and changelog generation.

By adopting this standard, you improve your communication skills and make your projects easier to maintain and scale.

---
## 🛠️ How to Use Conventional Commits

### Basic Structure

Each commit message follows this format:

```
<type>(<scope>): <description>

[optional body]

[optional footer]
```

- **type**: Describes the category of the change (e.g., `feat`, `fix`, `docs`).
- **scope**: (Optional) Specifies the area of the project affected (e.g., `auth`, `ui`, `api`).
- **description**: A concise summary of the change.
- **body**: (Optional) Provides additional context or details.
- **footer**: (Optional) Includes metadata like breaking changes or issue references.

---

## 🔥 Types of Commits with Examples

Here are the most common commit types, with examples:

### 1. **feat**: A new feature for the user or system
```
feat(auth): add Google login feature
feat(api): implement user search endpoint
```

### 2. **fix**: A bug fix
```
fix(button): resolve hover state issue
fix(api): correct typo in endpoint URL
```

### 3. **docs**: Documentation updates
```
docs(readme): update installation instructions
docs(api): add endpoint usage details
```

### 4. **style**: Code style changes (e.g., formatting, white-space)
```
style(navbar): fix alignment issues
style(css): remove unused styles
```

### 5. **refactor**: Code changes that neither fix bugs nor add features
```
refactor(auth): simplify login validation logic
refactor(ui): restructure folder hierarchy
```

### 6. **test**: Adding or updating tests
```
test(api): add tests for user search endpoint
test(auth): update login function tests
```

### 7. **chore**: Routine tasks or maintenance
```
chore(deps): update react to version 18.0.0
chore(lint): add ESLint rules for codebase
```

### 8. **build**: Changes that affect the build system or dependencies
```
build(webpack): configure production build
build(deps): add Babel plugin for optimization
```

### 9. **ci**: Continuous integration-related changes
```
ci(github): update GitHub Actions workflow
ci(jenkins): fix deployment pipeline script
```

---

## 🧑‍💻 Step-by-Step Workflow

### 1. **Make Your Changes**
Modify the files in your project as needed.

### 2. **Stage Your Changes**
Add your files to the staging area:

```bash
git add <file>
# Or to add all changes:
git add .
```

### 3. **Commit with a Conventional Commit Message**

Write a descriptive commit message following the format:

```bash
git commit -m "<type>(<scope>): <description>"
```

#### Examples:
```bash
git commit -m "feat(auth): add Google login feature"
git commit -m "fix(button): resolve hover state issue"
```

### 4. **Push Your Changes**
Push the changes to your remote repository:

```bash
git push origin <branch-name>
```

---

## 💡 Best Practices

1. **Be Concise but Descriptive**
   - Write commit messages that clearly describe what you did and why.

2. **Use the Correct Type**
   - Choose a type (`feat`, `fix`, `docs`, etc.) that best fits the change.

3. **Scope It**
   - Use scopes to specify the affected area of the project (e.g., `ui`, `api`).

4. **Breaking Changes**
   - Include `BREAKING CHANGE:` in the footer if the commit introduces a breaking change.

   Example:
   ```
   feat(auth): update login process

   BREAKING CHANGE: The login endpoint now requires an additional parameter.
   ```

5. **Reference Issues**
   - Use `Fixes #<issue-number>` or `Closes #<issue-number>` in the footer to link commits to issues.

   Example:
   ```
   fix(api): resolve null pointer exception in user search

   Fixes #42
   ```

6. **Atomic Commits**
   - Focus on one change per commit to make history easier to read and understand.

---

## 📘 Advanced Examples

### Adding Features
```bash
git commit -m "feat(api): add endpoint for user profile update"
git commit -m "feat(ui): implement dark mode toggle"
```

### Fixing Bugs
```bash
git commit -m "fix(auth): correct password hashing algorithm"
git commit -m "fix(ui): resolve crash on theme change"
```

### Updating Documentation
```bash
git commit -m "docs(readme): update API usage instructions"
git commit -m "docs(contributing): add code of conduct"
```

### Refactoring Code
```bash
git commit -m "refactor(auth): simplify JWT validation logic"
git commit -m "refactor(db): optimize query performance"
```

---

## 📚 Resources

For more details, refer to the official documentation: [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)

---

## 💡 Tips for Success

- **Automate Your Workflow**: Use tools like `commitlint` to enforce commit message conventions.
- **Leverage Git Hooks**: Set up pre-commit hooks to validate your messages before committing.
- **Keep Practicing**: The more you use Conventional Commits, the more natural it becomes.

Happy Committing! 🎉

