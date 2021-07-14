pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                //git 'https://github.com/sacindia/my-app.git'


                // To run Maven on a Windows agent, use
                //bat "mvn -Dmaven.test.failure.ignore=true clean package"
                bat "mvn clean"
            }

            }
        stage('Test') {
            steps {
                // To run Maven on a Windows agent, use
                bat "mvn test"
            }

            }
                    stage('Deploy') {
            steps {
                // To run Maven on a Windows agent, use
                bat "mvn package"
            }

            }
        }
    }
