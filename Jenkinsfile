pipeline{
    agent any

    stages{
        stage('checkout'){
            steps{
                checkout scm
            }
        }
    

    stage('install dependenies'){
        steps{
            sh '''
              npm install express mysql2 dotenv
            '''
        }
        stage('start the server'){
            steps{
                sh '''
                  node server.js
                  
                '''
                }
            }
        }
    }
}