pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/shashikala317/cicd-project.git'
            }
        }
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t cicd-app:latest .'
            }
        }
        stage('Run Container') {
            steps {
                sh 'docker run -d -p 8080:80 cicd-app:latest'
            }
        }
	stage('Run Container') {
 	    steps {
    		sh 'docker run -d -p 8080:80 cicd-app:latest'
	    }
	}
	
    }
}

