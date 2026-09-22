# GitHub Actions Demo

A minimal ASP.NET Core (.NET 10) web API used to demonstrate a basic CI pipeline with GitHub Actions.

## What's inside

- A single minimal-API endpoint (`GET /`) that returns `Hello World!`
- A GitHub Actions workflow (`.github/workflows/ci.yml`) that runs on every push and pull request:
  - Restores dependencies
  - Builds the project
  - Runs tests

## Requirements

- [.NET 10 SDK](https://dotnet.microsoft.com/download)

## Getting started

```bash
dotnet restore
dotnet run
```

The app will start on the URL shown in the console output (see `Properties/launchSettings.json`).

## Running tests

```bash
dotnet test
```

## CI

Every push and pull request triggers the `CI Pipeline` workflow defined in [`.github/workflows/ci.yml`](.github/workflows/ci.yml), which restores, builds, and tests the project on `ubuntu-latest`.
