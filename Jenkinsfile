pipeline {
    agent any

    environment {
        DOCKER_IMAGE = 'react-app'
        DOCKER_CONTAINER = 'react-container'
        STAGING_SERVER = 'staging.example.com'
        PRODUCTION_SERVER = 'production.example.com'
        EMAIL_RECIPIENT = 'ansh4764.be23@chitkara.edu.in'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building the React application...'
                echo 'Tools: npm, Webpack, Vite'
                echo 'Integration Steps: Install dependencies using npm, build the React app using Webpack or Vite, and generate optimized production assets.'
                echo 'What it does: Compiles React code into a minified, production-ready format.'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit and integration tests...'
                echo 'Tools: Jest, Mocha, React Testing Library'
                echo 'Integration Steps: Use Jest and React Testing Library to validate component functionality. Ensure test coverage meets project standards.'
                echo 'What it does: Tests individual React components and their integration with state and APIs.'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Performing static code analysis with ESLint and SonarQube...'
                echo 'Tools: ESLint, SonarQube, Prettier'
                echo 'Integration Steps: Run ESLint to check code style and SonarQube for static code analysis.'
                echo 'What it does: Ensures the code follows best practices and detects potential bugs.'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Running security scan with OWASP Dependency Check...'
                echo 'Tools: OWASP Dependency Check, Snyk, GitHub Dependabot'
                echo 'Integration Steps: Scan package dependencies for known vulnerabilities using OWASP Dependency Check.'
                echo 'What it does: Identifies security risks in project dependencies.'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Deploying React app to staging using Docker...'
                echo 'Tools: Docker, Kubernetes, Nginx'
                echo 'Integration Steps: Build a Docker image with the React app, run an Nginx container to serve it, and expose it on the staging server.'
                echo 'What it does: Deploys the React app inside a Docker container, making it accessible for testing.'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Running end-to-end tests on staging with Selenium...'
                echo 'Tools: Selenium, Cypress, Playwright'
                echo 'Integration Steps: Execute Selenium test cases against the staging URL to validate full application workflows.'
                echo 'What it does: Ensures that the deployed React app works correctly in the staging environment.'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Deploying React app to production using Docker...'
                echo 'Tools: Docker, Kubernetes, AWS ECS'
                echo 'Integration Steps: Build and tag the Docker image for production, push it to a registry (optional), and run an Nginx container to serve the React app.'
                echo 'What it does: Deploys the React app in a production-ready Docker container.'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully!'
            echo 'Tools: Jenkins, Slack, Prometheus'
            echo 'Integration Steps: Ensure successful execution of all pipeline stages, from build to production deployment.'
            echo 'What it does: Confirms the React app is built, tested, analyzed, scanned, and deployed correctly.'
        }
        failure {
            echo 'Pipeline failed! Check the logs for more details.'
            echo 'Tools: Jenkins, ELK Stack, Grafana'
            echo 'Integration Steps: Identify the failing stage, analyze logs, and troubleshoot errors for resolution.'
            echo 'What it does: Notifies the team of pipeline failures for immediate attention.'
        }
    }
}
