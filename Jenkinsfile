pipeline {
    agent any
  
    stages {
        stage('Build') {
            steps {
                sh 'pip3 install flask'
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
