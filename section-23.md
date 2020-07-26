## **Section 23: CI/CD**

## Table of Contents
- [**Section 23: CI/CD**](#section-23-cicd)
- [Table of Contents](#table-of-contents)
  - [Development Workflow](#development-workflow)
  - [Git Repository Approaches](#git-repository-approaches)
  - [Creating a GitHub Action](#creating-a-github-action)
  - [Adding a CI Test Script](#adding-a-ci-test-script)
  - [Running Tests on PR Creation](#running-tests-on-pr-creation)
  - [Output of Failing Tests](#output-of-failing-tests)
  - [Running Tests in Parallel](#running-tests-in-parallel)
  - [Verifying a Test Run](#verifying-a-test-run)
  - [Selective Test Execution](#selective-test-execution)
  - [Deployment Options](#deployment-options)
  - [Creating a Hosted Cluster](#creating-a-hosted-cluster)
  - [Reminder on Kubernetes Context](#reminder-on-kubernetes-context)
  - [Reminder on Swapping Contexts](#reminder-on-swapping-contexts)
  - [The Deployment Plan](#the-deployment-plan)
  - [Building an Image in an Action](#building-an-image-in-an-action)
  - [Testing the Image Build](#testing-the-image-build)
  - [Restarting the Deployment](#restarting-the-deployment)
  - [Applying Kubernetes Manifests](#applying-kubernetes-manifests)
  - [Prod vs Dev Manifest Files](#prod-vs-dev-manifest-files)
  - [Manual Secret Creation](#manual-secret-creation)
  - [Don't Forget Ingress-Nginx!](#dont-forget-ingress-nginx)
  - [Testing Automated Deployment](#testing-automated-deployment)
  - [Additional Deploy Files](#additional-deploy-files)
  - [A Successful Deploy!](#a-successful-deploy)
  - [Buying a Domain Name](#buying-a-domain-name)
  - [Configuring the Domain Name](#configuring-the-domain-name)
  - [One Small Fix](#one-small-fix)
  - [One More Small Fix](#one-more-small-fix)
  - [I Really Hope This Works](#i-really-hope-this-works)
  - [Next Steps](#next-steps)

### Development Workflow

![](section-23/teams.jpg)
![](section-23/branch.jpg)

**[⬆ back to top](#table-of-contents)**

### Git Repository Approaches
**[⬆ back to top](#table-of-contents)**

### Creating a GitHub Action
**[⬆ back to top](#table-of-contents)**

### Adding a CI Test Script
**[⬆ back to top](#table-of-contents)**

### Running Tests on PR Creation
**[⬆ back to top](#table-of-contents)**

### Output of Failing Tests
**[⬆ back to top](#table-of-contents)**

### Running Tests in Parallel
**[⬆ back to top](#table-of-contents)**

### Verifying a Test Run
**[⬆ back to top](#table-of-contents)**

### Selective Test Execution
**[⬆ back to top](#table-of-contents)**

### Deployment Options
**[⬆ back to top](#table-of-contents)**

### Creating a Hosted Cluster
**[⬆ back to top](#table-of-contents)**

### Reminder on Kubernetes Context
**[⬆ back to top](#table-of-contents)**

### Reminder on Swapping Contexts
**[⬆ back to top](#table-of-contents)**

### The Deployment Plan
**[⬆ back to top](#table-of-contents)**

### Building an Image in an Action
**[⬆ back to top](#table-of-contents)**

### Testing the Image Build
**[⬆ back to top](#table-of-contents)**

### Restarting the Deployment
**[⬆ back to top](#table-of-contents)**

### Applying Kubernetes Manifests
**[⬆ back to top](#table-of-contents)**

### Prod vs Dev Manifest Files
**[⬆ back to top](#table-of-contents)**

### Manual Secret Creation
**[⬆ back to top](#table-of-contents)**

### Don't Forget Ingress-Nginx!
**[⬆ back to top](#table-of-contents)**

### Testing Automated Deployment
**[⬆ back to top](#table-of-contents)**

### Additional Deploy Files
**[⬆ back to top](#table-of-contents)**

### A Successful Deploy!
**[⬆ back to top](#table-of-contents)**

### Buying a Domain Name
**[⬆ back to top](#table-of-contents)**

### Configuring the Domain Name
**[⬆ back to top](#table-of-contents)**

### One Small Fix
**[⬆ back to top](#table-of-contents)**

### One More Small Fix
**[⬆ back to top](#table-of-contents)**

### I Really Hope This Works
**[⬆ back to top](#table-of-contents)**

### Next Steps
**[⬆ back to top](#table-of-contents)**