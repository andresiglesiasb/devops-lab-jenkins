# devops-lab-jenkins: Declarative Pipeline

![Jenkins](https://img.shields.io/badge/Jenkins-2.0+-red.svg) ![Status](https://img.shields.io/badge/Status-Educational-blue.svg)

## Overview
This repository contains the **Infrastructure as Code (IaC)** configuration for a Continuous Integration pipeline. It demonstrates the transition from manual "Freestyle" jobs to modern **Declarative Pipelines** using a `Jenkinsfile`.

The goal of this project is to simulate a standard CI/CD workflow including Build, Test, and Deploy stages, orchestrated automatically by a Jenkins server.

## Key Features
* **Pipeline as Code:** All build logic is versioned in Git (Groovy syntax).
* **Declarative Syntax:** Uses the modern, readable Jenkins structure (`pipeline { ... }`).
* **Multi-Stage Workflow:** clearly defined stages for:
    * 🛠 **Build:** Simulates code compilation.
    * ✅ **Test:** Simulates unit testing execution.
    * 🚀 **Deploy:** Simulates deployment to a staging environment.

## Pipeline Structure
The pipeline is defined in the `Jenkinsfile` and follows this logic:

```groovy
pipeline {
    agent any // Runs on any available node (currently the built-in node)

    stages {
        stage('Build') { ... }
        stage('Test')  { ... }
        stage('Deploy'){ ... }
    }
}
