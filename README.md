# Node.js Application with SCA Scanning

This repository contains a sample Node.js application integrated with a GitHub Actions workflow for Software Composition Analysis (SCA) using Snyk.

## Purpose

The primary objective of this project is to demonstrate how to integrate SCA into your CI/CD pipeline using GitHub Actions. The workflow automatically scans project dependencies for vulnerabilities using Snyk.

## Project Structure

- `index.js`: The main Node.js application file.
- `package.json`: Defines project dependencies.
- `.github/workflows/sca-scan.yml`: GitHub Actions workflow for running SCA with Snyk.
- `README.md`: Documentation about the project and its SCA setup.

## GitHub Actions Workflow

The `.github/workflows/sca-scan.yml` file defines a GitHub Actions workflow to:

1. **Checkout Code**: Retrieve the latest code from the repository.
2. **Set Up Node.js**: Install the specified version of Node.js.
3. **Install Dependencies**: Run `npm install` to install dependencies.
4. **Install Snyk CLI**: Install Snyk for vulnerability scanning.
5. **Run Snyk Test**: Perform a scan of project dependencies to identify vulnerabilities.
