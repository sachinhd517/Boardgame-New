pipeline {    
    agent { label 'agent-1' }
    tools {
        jdk 'jdk17'
        maven 'maven 3.8.6'
    }

    stages {   
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}


