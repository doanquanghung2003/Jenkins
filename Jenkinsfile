pipeline {
    agent any 
    stages{
        stage('Clone') {
            steps {
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/doanquanghung2003/Jenkins.git'
            }
        }
    }
}