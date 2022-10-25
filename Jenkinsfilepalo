pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('integrationTest') {
            	agent {
                	docker { image 'maven:3.8.1-adoptopenjdk-11' }
            }
            steps {
                sh 'echo "inside the container" && sleep 20'
            }
    }
            }
        }
