pipeline {
    agent any
    
    stages {
        
        stage('checkout') {
            steps {
                git branch: 'main', poll: false, url: 'https://github.com/srinugit11/myfirstrepo.git'
            }
        
        }
        stage("dev") {
            
            steps {
                sh "echo 'devlopment stage'"
                sh "/home/srinu/srinu/dev.sh"
                
            }
            
            
        }
        
        
        stage('test'){
            
            steps {
                sh "echo 'test stage'"
                sh "/home/srinu/srinu/test.sh"
            }
            
            
        }
        
        
        stage('production') {
            
            steps {
                sh "echo 'production stage'"
                sh "/home/srinu/srinu/prod.sh"
            }
            
        }
    }
}
