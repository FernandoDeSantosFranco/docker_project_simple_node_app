pipeline {
    agent any
    
    stages {
        stage('Clone repo') {
            steps {
                git branch: 'main', url: 'https://github.com/FernandoDeSantosFranco/docker_project_simple_node_app.git'
            }
        }
        
        stage('Build docker image') {
            steps {
                script {
                    sh 'pwd'
                    docker.build('ferfranco01/node-app:latest')
                }
            }
        }
    }
}