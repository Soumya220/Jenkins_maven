pipeline {
    agent any 
    stages {
        stage('Clone Repository') { 
            steps {
                sh "git clone https://github.com/Soumya220/Jenkins_maven.git" 
                sh "mvn clean"
            }
        }
        stage('Test ') { 
            steps {
               sh "mvn test" 
                }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package" 
            }
       }
    }
}
