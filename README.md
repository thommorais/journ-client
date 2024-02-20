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
   git clone https://github.com/your-organization/journ-client.git
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
