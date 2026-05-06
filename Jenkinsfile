pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Using Maven to compile and package code..."
                echo "Success!"
            }
        }
        stage('Test') {
            steps {
                echo "Running unit test using Jest..."
                sleep (1)
                echo "Success!"
                echo "Running intergration test using Postman..."
                sleep (1)
                echo "Success!"

            }
        }
        stage('Code Analysis') {
            steps {
                echo "Using Biome to make sure code meets industry standards..."
                sleep (1)
                echo "Success!"

            }
        }
        stage('Security Scan') {
            steps {
                echo "Scanning for vulnerailitys using OWASP Dependancy-Check..."
                sleep (2)
                echo "Success!"
            }
        }
        stage('Deploy to staging') {
            steps {
                echo "Deploying to staging server... Using AWS EC2 instance"
                sleep (1)
                echo "Success"
                }
        }
        stage('Intergration Tests on staging') {
            steps {
                echo "Running intergration tests on staging enviroment"
                echo "Success! Application funtions as intended"
            }
        }
        stage('Deploy to Production') {
            steps {
                echo "Deploying application to production server..."
                sleep (4)
                echo "Success! Application deployed"
            }
        }

    }
}
