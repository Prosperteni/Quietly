# Contributing to Quietly

First off, thank you for considering contributing to Quietly! It's people like you that make Quietly such a great extension.

This document provides guidelines and instructions on how you can contribute to this project. 

## Getting Started

1. **Fork the repository** on GitHub.
2. **Clone your fork** to your local machine:
   ```bash
   git clone https://github.com/YOUR-USERNAME/Quietly.git
   cd Quietly
   ```
3. **Add the original repository** as a remote to sync updates:
   ```bash
   git remote add upstream https://github.com/Prosperteni/Quietly.git
   ```

## Branching Strategy

Please create a new branch for each feature, bug fix, or documentation update you are working on. Do not commit directly to the `main` branch.

Use descriptive branch names. We recommend the following prefixes:
- `feature/` or `feat/` for new features (e.g., `feat/improve-ad-detection`)
- `bugfix/` or `fix/` for bug fixes (e.g., `fix/popup-styling`)
- `docs/` for documentation updates (e.g., `docs/update-readme`)

```bash
git checkout -b feat/your-new-feature
```

## Making Changes & Testing Locally

Since Quietly is a Chrome extension, you can easily test your changes locally in developer mode.

1. Open **Chrome** and navigate to `chrome://extensions/`.
2. Enable **Developer mode** using the toggle in the top right corner.
3. Click **Load unpacked** and select the `Quietly` project directory.
4. Open a YouTube video with an ad to verify your changes.

**Note:** If you make changes to the code (`background.js`, `content.js`, `popup.js`, etc.) while the extension is loaded, you will need to click the **Refresh** icon (⟳) on the Quietly extension card in `chrome://extensions/` and refresh your open YouTube tabs to see the updates in effect.

## Commit Message Format

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification for our commit messages. This leads to more readable messages that are easy to follow.

Format:
```
<type>: <short description>
```

Examples:
- `feat: add support for skipping new ad format`
- `fix: resolve popup UI glitch on macOS`
- `docs: update contributing section`
- `refactor: optimize ad detection loop`

**Types:**
- `feat`: A new feature
- `fix`: A bug fix
- `docs`: Documentation only changes
- `style`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
- `refactor`: A code change that neither fixes a bug nor adds a feature
- `test`: Adding missing tests or correcting existing tests
- `chore`: Changes to the build process or auxiliary tools and libraries

## Submitting a Pull Request

When you are ready to submit your changes:

1. **Push your branch** to your forked repository:
   ```bash
   git push origin feat/your-new-feature
   ```
2. Open a **Pull Request (PR)** on the original [Quietly repository](https://github.com/Prosperteni/Quietly).
3. Provide a clear and descriptive title for your PR.
4. Explain the changes you made, why you made them, and any related issues (e.g., "Fixes #123").
5. Wait for a maintainer to review your PR. They may ask for some changes before it gets merged.

---

**We look forward to seeing your contributions!**
