# Playwright Website Testing Project

A TypeScript-based Playwright testing project for automated website testing.

## Prerequisites

- Node.js (v18 or higher)
- npm

## Installation

```bash
npm install
```

## Running Tests

```bash
# Run all tests
npm test

# Run tests in headed mode (see browser)
npm run test:headed

# Run tests in UI mode (interactive)
npm run test:ui

# Run tests in debug mode
npm run test:debug

# Show test report
npm run report
```

## Project Structure

```
.
├── tests/              # Test files
│   └── example.spec.ts # Example test
├── playwright.config.ts # Playwright configuration
├── tsconfig.json       # TypeScript configuration
└── package.json        # Project dependencies
```

## Configuration

The Playwright configuration is in [playwright.config.ts](playwright.config.ts). It includes:
- Test directory: `./tests`
- Browsers: Chromium, Firefox, WebKit
- Parallel execution enabled
- HTML reporter

## Writing Tests

Tests are written in TypeScript. Example:

```typescript
import { test, expect } from '@playwright/test';

test('example test', async ({ page }) => {
  await page.goto('https://example.com');
  await expect(page).toHaveTitle(/Example/);
});
```

## GitHub Repository

This project is connected to GitHub. To push changes:

```bash
git add .
git commit -m "Your commit message"
git push
```
