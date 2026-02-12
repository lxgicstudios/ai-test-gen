# ai-test-gen

[![npm version](https://img.shields.io/npm/v/@lxgicstudios/ai-test-gen.svg)](https://www.npmjs.com/package/@lxgicstudios/ai-test-gen)
[![npm downloads](https://img.shields.io/npm/dm/@lxgicstudios/ai-test-gen.svg)](https://www.npmjs.com/package/@lxgicstudios/ai-test-gen)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js](https://img.shields.io/badge/node-%3E%3D18-brightgreen)](https://nodejs.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-Ready-blue.svg)](https://www.typescriptlang.org/)

Point it at your source files and it writes unit tests for you. Supports Jest, Vitest, and Mocha.

## Quick Start

```bash
npx @lxgicstudios/ai-test-gen src/utils.ts --framework jest
```

## Setup

```bash
export OPENAI_API_KEY=sk-your-key-here
```

## Usage

```bash
# Generate Jest tests for a file
npx @lxgicstudios/ai-test-gen src/utils.ts --framework jest

# Vitest instead
npx @lxgicstudios/ai-test-gen src/utils.ts --framework vitest

# Multiple files
npx @lxgicstudios/ai-test-gen "src/**/*.ts" --framework jest

# Save to a file
npx @lxgicstudios/ai-test-gen src/utils.ts --framework jest -o src/__tests__/utils.test.ts
```

## What you get

Actual test files with imports, describe blocks, and test cases. It covers happy paths, edge cases, and error handling. You'll probably want to tweak them a bit, but it beats starting from scratch.

## Supported Frameworks

- **Jest** - Meta's testing framework
- **Vitest** - Vite-native unit testing
- **Mocha** - Flexible test runner

## Why use ai-test-gen?

- Generates test scaffolding in seconds
- Understands TypeScript types and function signatures
- Creates edge case tests you'd forget
- Gets you 80% there so you can focus on the tricky parts

## Heads up

The generated tests are a starting point. They won't know about your mocks, test utilities, or specific setup. But they'll get you 80% there, which is the annoying part anyway.

## License

MIT — Built by [LXGIC Studios](https://github.com/lxgicstudios)
