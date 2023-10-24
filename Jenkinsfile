pipeline {
    agent any
    stages {
        stage('checkout') {
        
            
            steps {
		sh 'rm -rf hello-world-war'
                sh 'git clone https://github.com/ASLAMBASHA1539/hello-world-war.git'
            }
        }
	stage('Build') {
        
            
            steps {
		sh 'mvn clean package'
            }
        }
    }
}
