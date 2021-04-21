pipeline {
    agent any
  
    stages {
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') {
            steps {
                sh 'python3 app.py'
            }
        }
    }
}
