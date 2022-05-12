pipeline {
    agent any
   
    stages {
        
         stage('start stage') {
            steps {
                echo "Logging start stage"    
            }
        }
  
        // Building Docker images
        stage('Building image') {
            steps {
                script {
                    dockerImage = docker.build "sample_image:123"
                }
            }
        }
   
        // Uploading Docker images into AWS ECR
        stage('Pushing to ECR') {
            steps{  
                echo "Pushing stage"
            }
        }
    }
}
