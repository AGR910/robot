pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
            	echo 'Building....'
                sh 'mvn clean install'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh 'cp target/robot.war /webapps'
            }
        }
    }
}