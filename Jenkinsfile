pipeline {
    agent {
        dockerContainer {
            image 'maven:3.9.0'
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}