# Commit Message Cheatsheet (Conventional Commits)

## Types

### 🚀 feat
- **Meaning**: A new feature for the user.
- **Example**:
  ```
  feat(terminal): add dark theme switcher
  ```

### 🐞 fix
- **Meaning**: A bug fix.
- **Example**:
  ```
  fix(ui): prevent crash when navigation frame is empty
  ```

### 📖 docs
- **Meaning**: Documentation only changes (README, comments, wikis).
- **Example**:
  ```
  docs(readme): add quick start instructions
  ```

### 🎨 style
- **Meaning**: Code style, formatting, no logic changes (tabs, spaces, semicolons).
- **Example**:
  ```
  style(xaml): reformat titlebar indentation
  ```

### 🔧 refactor
- **Meaning**: Code changes that neither fix a bug nor add a feature.
- **Example**:
  ```
  refactor(app): simplify theme manager init
  ```

### ⚡ perf
- **Meaning**: Performance improvements.
- **Example**:
  ```
  perf(viewmodels): reduce allocations in UpdateLoop
  ```

### ✅ test
- **Meaning**: Adding or fixing tests.
- **Example**:
  ```
  test(settings): add unit tests for theme switching
  ```

### 🏗️ build
- **Meaning**: Build system or dependencies changes (NuGet, SDK, MSBuild).
- **Example**:
  ```
  build: bump WPF-UI to 4.0.3
  ```

### 🔄 ci
- **Meaning**: Continuous Integration files (GitHub Actions, pipelines).
- **Example**:
  ```
  ci(github): cache nuget packages in workflow
  ```

### 🧹 chore
- **Meaning**: Maintenance tasks (no code logic): configs, tools, cleanup.
- **Example**:
  ```
  chore(repo): add CODEOWNERS and issue templates
  ```

### ⏪ revert
- **Meaning**: Revert a previous commit.
- **Example**:
  ```
  revert: feat(terminal): add dark theme switcher
  ```

---

## BREAKING CHANGE

If the change is not backward compatible, add a BREAKING CHANGE section in the body:

```
feat(settings): replace theme enum with ThemeManager

BREAKING CHANGE: Theme enum was removed, use ThemeManager instead
```

---

## Scope

The scope (in parentheses) indicates the part of the project affected.

Examples: `terminal`, `ui`, `build`, `ci`, `readme`, `deps`, `github`.

---

## Summary

Always start commit with:

```
<type>(<scope>): <short summary>
```

Keep the summary short and meaningful (max ~72 chars).

