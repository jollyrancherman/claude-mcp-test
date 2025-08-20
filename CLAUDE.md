# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

# Core Development Philosophy

## KISS (Keep It Simple, Stupid)

Simplicity should be a key goal in design. Choose straightforward solutions over complex ones whenever possible. Simple solutions are easier to understand, maintain, and debug.

## YAGNI (You Aren't Gonna Need It)

Avoid building functionality on speculation. Implement features only when they are needed, not when you anticipate they might be useful in the future.

## Design Principles

Dependency Inversion: High-level modules should not depend on low-level modules. Both should depend on abstractions.
Open/Closed Principle: Software entities should be open for extension but closed for modification.
Single Responsibility: Each function, class, and module should have one clear purpose.
Fail Fast: Check for potential errors early and raise exceptions immediately when issues occur.

# Code Structure & Modularity

## File and Function Limits

Never create a file longer than 500 lines of code. If approaching this limit, refactor by splitting into modules.
Functions should be under 50 lines with a single, clear responsibility.
Classes should be under 100 lines and represent a single concept or entity.
Organize code into clearly separated modules, grouped by feature or responsibility.
Line lenght should be max 100 characters ruff rule in pyproject.toml
Use venv_linux (the virtual environment) whenever executing Python commands, including for unit tests.

## Project Overview

A Next.js application called "focus" built with TypeScript, Tailwind CSS, shadcn/ui, and ESLint. The project uses the App Router architecture and organizes code within a `src/` directory. UI components are built using the shadcn/ui component library for a consistent, accessible design system.

## Development Commands

```bash
cd focus
npm run dev      # Start development server on http://localhost:3000
npm run build    # Build production application
npm run start    # Start production server
npm run lint     # Run ESLint for code quality checks

# shadcn/ui component management
npx shadcn@latest add [component]  # Add a new shadcn component
npx shadcn@latest diff [component] # Check for component updates
```

## Architecture

To be documented as the project structure emerges.
