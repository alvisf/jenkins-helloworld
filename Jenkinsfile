pipeline {
    agent any
  
    stages {
        stage('Build') {
            steps {
                sh 'sudo pip3 install flask'
            }
        }
        stage('Distroy') {
            steps {
                sh 'sudo kill $(sudo lsof -t -i:80)'
            }
        }
        stage('Next') {
            steps {
                sh ''
            }
        }
        stage('Deploy') {
            steps {
                sh 'sudo nohup python3 app.py &'
                
            }
        }
    }
}
