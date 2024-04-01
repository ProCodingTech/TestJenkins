pipeline {

    agent any
    
    stages {
         stage('install') {
          steps {
              sh 'npm install'
            }
          }
          stage('start') {
          steps {
              sh 'npm start'
            }
          }
        
        stage('test') {
          steps {
              sh 'echo test'
            }
          }
          stage('Docker Image') {
          steps {
              sh 'docker build -t SCDLABTASK'
            }
          }
        
        stage('Docker Comopse Up') {
            steps {
               
                    sh "docker compose up"
                
            }
        }
    }
}
