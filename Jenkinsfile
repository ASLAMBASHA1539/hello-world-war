pipeline {
	agent none
    stages {
        stage('checkout') {
        agent { label 'slave1' }
            
            steps {
		sh 'rm -rf hello-world-war'
                sh 'git clone https://github.com/ASLAMBASHA1539/hello-world-war.git'
            }
        }
	stage('Build') {
        
            agent { label 'slave1' }
            steps {
		sh 'mvn clean package'
            }
        }
    }
}
