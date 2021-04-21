pipeline {
    agent any
  
    stages {
        stage('Build') {
            steps {
                sh 'sudo pip3 install flask'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') {
            steps {
                sh 'sudo python3 app.py >> log.txt 2>&1 &'
            }
        }
    }
}
