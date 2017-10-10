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
                  if(isUnix()){
						sh 'gradle build --info'
					  }
					  else{
						bat 'gradle build --info'
					  }
            }
        }
    }
}