# Node.js CI/CD Pipeline

## Overview

This project implements a Continuous Integration / Continuous Deployment (CI/CD) pipeline for a Node.js application using Jenkins and a set of related tools. The pipeline includes steps for building, testing, containerization, security scanning, and deployment.

## Tools Used

- **Jenkins:** The automation server for building, testing, and deploying the Node.js application.

- **Docker:** Used for containerizing the Node.js application, providing consistency across different environments.

- **SonarQube:** Used for static code analysis to identify and fix code quality issues.

- **Trivy:** Used for scanning Docker images to identify and fix vulnerabilities.

- **OWASP Dependency-Check:** Used for checking dependencies for known vulnerabilities.

## CI/CD Pipeline Steps

1. **Build:**
   - Jenkins automatically triggers a build on code changes.
   - Node.js application is built from source code.

2. **Test:**
   - Automated tests are executed to ensure code quality and functionality.

3. **Containerization:**
   - The application is containerized using Docker for portability and consistency.

4. **Security Scanning:**
   - SonarQube performs static code analysis to identify code quality issues.
   - Trivy scans the Docker image for vulnerabilities.
   - OWASP Dependency-Check checks dependencies for known vulnerabilities.

5. **Deployment:**
   - Deployment to a staging or production environment is triggered based on successful tests and security scans.


