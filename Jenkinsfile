pipeline {
    agent any
    
   
    
    stages {
       
        
        stage('Build') {
            steps {
                // Your build steps here
                sh 'echo "Building..."'
                sh 'ls'
                echo ${params.env}
            }
        }
        
        stage('Test') {
            steps {
                // Your test steps here
                sh 'echo "Testing..."'
            }
        }
        
        stage('Deploy') {
            steps {
                // Your deployment steps here
                sh 'echo "Deploying..."'
            }
        }
    }
    
    post {
        success {
            script {
                echo "Pipeline succeeded!"
            }
        }
        failure {
            script {
                echo "Pipeline failed!"
            }
        }
    }
}