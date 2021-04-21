pipeline {

    agent any
   
    stages {
        stage('Compile stage') {
            steps {
                echo "mvn clean compile" 
        }
    }

         stage('testing stage') {
             steps {
                echo "mvn test"
        }
    }

          stage('deployment stage') {
              steps {
                python app.py
        }
    }

  }

}
