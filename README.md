# Playwright Test Suite

This repository contains automated tests built with [Playwright](https://playwright.dev/), a modern end-to-end testing framework.

## Project Structure

- **tests/** - Test specifications
  - `example.spec.ts` - Example test cases
- **playwright.config.ts** - Playwright configuration
- **playwright-report/** - Test execution reports
- **test-results/** - Test result artifacts
- **.github/workflows/** - CI/CD workflows
  - `playwright.yml` - GitHub Actions workflow for running tests

## Prerequisites

- Node.js (v14 or higher)
- npm or yarn

## Installation

Install dependencies:

```bash
npm install
```

## Running Tests

Run all tests:

```bash
npm test
```

Run tests in UI mode:

```bash
npm run test:ui
```

Run tests in debug mode:

```bash
npm run test:debug
```

## Configuration

Test configuration is defined in [playwright.config.ts](playwright.config.ts). This includes:
- Browser types (Chromium, Firefox, WebKit)
- Test timeout settings
- Report generation
- Base URL configuration

## CI/CD

Tests are automatically run via GitHub Actions. See [.github/workflows/playwright.yml](.github/workflows/playwright.yml) for workflow configuration.

## Reports

After running tests, view the HTML report:

```bash
npx playwright show-report
```

## License

See [.gitignore](.gitignore) for ignored files.