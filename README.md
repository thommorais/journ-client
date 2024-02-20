# Journ

This repository hosts the frontend applications and shared packages for Journ, a comprehensive productivity suite designed to streamline scheduling, task management, time tracking, and journaling. The suite is aimed at enhancing user productivity through a unified interface for web and macOS platforms.

## Overview

The Journ frontend monorepo is structured to facilitate the development of web and macOS applications, ensuring a cohesive user experience across platforms. The monorepo includes:

### Applications

- **/apps/web**: Contains the source code for the Journ web application, offering full access to all Journ features including scheduling, task management, time tracking, and journaling.

### Shared Packages

- **/packages/eslint-config**: Provides ESLint configuration settings shared across all frontend applications and packages to ensure code quality and consistency.

- **/packages/typescript-config**: Contains shared TypeScript configuration for maintaining strong typing and reducing errors during development.

- **/packages/ui**: Hosts reusable UI components that can be utilized across different parts of the Journ applications, promoting a consistent look and feel.

### Planned Applications

- **macOS Apps**: Future development includes macOS applications focused on time tracking and a comprehensive app that integrates all Journ features, aligning with the suite's core functionalities.

## Key Features

Journ's frontend applications aim to deliver:

- **Unified Productivity Suite**: A single platform that integrates essential productivity tools.
- **Clear Time Management**: Visual indicators and integrations for managing schedules and tasks.
- **Customizable User Experience**: Personalized settings to match individual preferences and productivity styles.
- **Efficiency and Focus**: Tools designed to prioritize tasks and manage deadlines effectively.

## Project Structure

The monorepo is organized to support efficient development workflows and shared resource management:

```
root/
├── apps/
│   └── web
└── packages/
    ├── eslint-config
    ├── typescript-config
    └── ui
```

## Getting Started

Prerequisites for development include:

- Node.js and npm or Yarn (for dependency management and script execution)
- A suitable IDE (e.g., Visual Studio Code) with support for ESLint and TypeScript

To set up the project:

1. Clone the repository:
```sh
   git clone https://github.com/thommorais/journ-client.git
```

2. Install dependencies:
```sh
   cd journ-client
   pnpm install
```

3. Start the development server for the web application:
```sh
    pnpm dev:web
```

The web application will be accessible at `http://localhost:3000`.


---

## Branching Strategy

This project employs the Gitflow Workflow to streamline development and release processes. This approach separates development efforts from released code, ensuring stability and systematic updates.

### Key Branches

- **`main`**: Holds the release history. It's stable and reflects the production-ready state.
- **`develop`**: Serves as the integration branch for features, forming the basis for each release.

### Supporting Branches

- **Feature Branches (`feature/*`)**: For developing new features. They originate from and merge back into `develop`.
- **Release Branches (`release/*`)**: Prepares for a new release, branching from `develop` and merging into `main` and back into `develop`.
- **Hotfix Branches (`hotfix/*`)**: Addresses urgent issues in the production version, branching from `main` and merging back into both `main` and `develop`.

### Workflow Overview

1. Develop features in `feature/*` branches, then merge into `develop`.
2. Create `release/*` branches from `develop` for release preparation.
3. Merge `release/*` branches into `main` for deployment, then back into `develop`.
4. Address production issues in `hotfix/*` branches, merging into both `main` and `develop`.

### Guidelines

- Merges into `develop` and `main` require pull requests for review.
- Naming conventions:
  - Feature: `feature/issue-#-description`
  - Release: `release/vX.Y.Z`
  - Hotfix: `hotfix/issue-#-description`

This strategy ensures a clear separation between ongoing development and stable releases, facilitating a structured and efficient workflow.

---

## Commit Convention

We follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) standard for commit messages, ensuring a clear and automated workflow.

### Format

Commit messages are structured as follows:

```
<type>[optional scope]: <description>
```

- **Type**: Describes the kind of change (e.g., `feat`, `fix`).
- **Scope** (optional): Denotes the part of the codebase affected.
- **Description**: Summarizes the change succinctly.

### Types

- `feat`: New features.
- `fix`: Bug fixes.
- Others include `docs`, `style`, `refactor`, `perf`, `test`, and `chore`.

### Benefits

- Enables automated versioning and changelog generation.
- Facilitates understanding of the project's history.

Contributors are expected to use this standardized format for all commits.