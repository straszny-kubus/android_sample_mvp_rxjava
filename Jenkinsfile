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
        stage('prebuild') {
            steps {
				script {
				  if(isUnix()){
					sh 'gradle --version'
				  } else{
					bat 'gradle --version'
				  }
				}
            }
        }
    }
}