pipeline {
    agent any

stages{
        stage('Build'){
            steps {
                sh 'mvn clean package'
                sh "docker build . tomcatwebapp:${env.BUILD_ID}"
            }
        }
    }
}
