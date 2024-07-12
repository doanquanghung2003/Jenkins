pipeline {
    agent any 
    stages{
        stage('Clone') {
            steps {
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/doanquanghung2003/Jenkins.git'
            }
        }
        stage('Push Docker Hub'){
            steps{
                // This step should not normally be used in your script. Consult the inline help for details.
                withDockerRegistry(credentialsId: '2f8dc1d6-7bb5-4003-a327-be19ed3bd896') {
                    // some block
                    // sh label: '', script: 'docker build -t doanhung9723/my-devops:latest .'
                    // sh label: '', script: 'docker push doanhung9723/my-devops:latest'
                     sh label: '', script: 'docker pull doanhung9723/my-devops:latest'
                }
            }
        }
    }
}