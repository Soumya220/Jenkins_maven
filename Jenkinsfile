pipeline {
    agent any 
    stages {
        stage('Clone Repository') { 
            steps {
                bat "git clone https://github.com/Soumya220/Jenkins_maven.git" 
                bat "mvn clean"
            }
        }
        stage('Test ') { 
            steps {
               bat "mvn test" 
                }
        }
        stage('Deploy') { 
            steps {
                bat "mvn package" 
            }
       }
    }
}
