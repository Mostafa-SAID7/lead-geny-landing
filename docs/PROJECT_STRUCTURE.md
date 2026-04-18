# Project Structure

## Overview

This is an Angular 21 application with a modern architecture following best practices.

## Directory Structure

```
lead-gen-landing/
├── src/
│   ├── app/              # Application components and modules
│   ├── assets/           # Static assets (images, fonts, etc.)
│   ├── environments/     # Environment configurations
│   └── styles/           # Global styles
├── docs/                 # Documentation files
├── screenshots/          # Application screenshots
├── .github/              # GitHub workflows and templates
├── dist/                 # Build output (generated)
├── node_modules/         # Dependencies (generated)
├── netlify.toml          # Netlify configuration
├── angular.json          # Angular CLI configuration
├── package.json          # Project dependencies
└── tsconfig.json         # TypeScript configuration
```

## Key Files

- **angular.json**: Angular workspace configuration
- **package.json**: Project metadata and dependencies
- **netlify.toml**: Netlify deployment configuration
- **tsconfig.json**: TypeScript compiler options

## Build Output

The build process generates files in `dist/lead-gen-landing/browser/` which is served by Netlify.
