pipeline {
    agent any
	tools {
        gradle 'gradle-3.2' 
    }
    stages {
        stage('przywitaj sie') {
            steps {
                echo "---!!!!!!-------- JESTEM!!!!!"
            }
        }
        stage('build') {
            steps {
                sh 'gradle --version'
            }
        }
    }
}