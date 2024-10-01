@Library("Shared") _
pipeline {
    agent {label "vinod"}

    stages {
        
        stage('Hello'){
            steps{
                script{
                    hello()
                }
            }
        }
        stage('Code') {
            steps {
                script{
                 clone("https://github.com/ritikasharma1505/django-notes-app.git", "main")
                }
            }
        }
        
        stage('Build') {
            steps {
              script{
                docker_build("notes-app","latest","ritikasharma1505")
              }
            }
        }
        
        stage('Push to DockerHub') {
            steps {
                script{
                    docker_push("notes-app","latest","ritikasharma1505")
                }
        
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'This is deploy process'
                sh 'docker compose up -d'
            }
        }
    }
}
