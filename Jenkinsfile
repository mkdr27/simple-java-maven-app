pipeline {
    agent any
    tools {
        maven 'Maven 3.9.7'
        jdk 'Java 17.0.6-ea'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package -Denforcer.skip=true' 
            }
        }
    }
}

