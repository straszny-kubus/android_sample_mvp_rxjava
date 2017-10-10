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
				script {
				  if(isUnix()){
					sh 'gradle build --info'
				  } else{
					bat 'gradle build --info'
				  }
				}
            }
        }
    }
}