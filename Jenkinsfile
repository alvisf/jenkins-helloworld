pipeline {
    agent any
  
    stages {
        stage('Build') {
            steps {
                sh 'sudo pip3 install flask'
            }
        }
        
        try{
            stage('Distroy') {
                sh 'sudo kill $(sudo lsof -t -i:80)' 
            }
        } catch(e) {
            echo e.toString()  
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
