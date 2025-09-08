pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo '''
                Task: Compile and package the source code into an executable format.
                Tool: Maven (commonly used build automation tool).
                '''
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo '''
                Task: Execute unit tests to validate individual functions and run integration tests 
                to verify that components interact correctly.
                Tools: JUnit for unit testing, TestNG for integration testing.
                '''
            }
        }

        stage('Code Analysis') {
            steps {
                echo '''
                Task: Perform static analysis on the codebase to detect issues, enforce coding standards, 
                and highlight maintainability concerns.
                Tool: SonarQube (industry-standard static code analysis tool).
                '''
            }
        }

        stage('Security Scan') {
            steps {
                echo '''
                Task: Assess the code and its dependencies for vulnerabilities to reduce security risks.
                Tool: OWASP Dependency-Check (Software Composition Analysis tool).
                '''
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo '''
                Task: Push the application package to a staging environment that mirrors production.
                Tool: Ansible (automation and deployment tool).
                '''
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo '''
                Task: Run automated integration tests against the application in the staging setup 
                to ensure it behaves as expected in a production-like environment.
                Tool: Selenium (integration and end-to-end testing tool).
                '''
            }
        }

        stage('Deploy to Production') {
            steps {
                echo '''
                Task: Release the verified application into the production environment.
                Tool: Ansible (used again for production deployment) .
                '''
            }
        }

    }
}

