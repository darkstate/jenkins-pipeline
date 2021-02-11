pipeline {
    agent any
    
    environment {
        PROJECT_NAME = "MyProj"
        OWNER_NAME = "MyName"
    }

    stages {
        stage('1-Build') {
            steps {
                echo 'Start of Stage Build'
                echo 'Building............'
                echo 'End of Stage Build'
            }
        }
        stage('2-Test') {
            steps {
                echo 'Start of Stage Test'
                echo "Hello ${OWNER_NAME} on project ${PROJECT_NAME}"
                echo 'Testing............'
                sh    "ls -la"
                echo 'End of Stage Test'
            }
        }
        stage('3-Deploy') {
            steps {
                echo 'Start of stage Deploy'
                echo 'Deploying............'
                sh '''
                ls -l
                pwd
                whoami
                '''
                sh "python --version"
                echo 'End of stage Deploy'
            }
        }
    }
}
