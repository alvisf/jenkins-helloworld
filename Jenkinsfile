pipeline {
    agent any
  
    stages {
        stage('Build') {
            steps {
                sh 'sudo pip3 install flask'
            }
        }
        
 
        
        stage('Deploy') {
            steps {
                sh 'sudo nohup python3 app.py &'
                
            }
        }
    }
}
