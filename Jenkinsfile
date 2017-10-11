pipeline {
    agent any
	tools {
        gradle 'gradle-3.2' 
    }
    stages {
        stage('przywitaj sie') {
            steps {
                echo "---!!!!!!-------- JESTEM!!!!! 2. raz.........."
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
	
	 post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if successful'
        }
        failure {
            echo 'This will run only if failed'
        }
        unstable {
            echo 'This will run only if the run was marked as unstable'
        }
        changed {
            echo 'This will run only if the state of the Pipeline has changed'
            echo 'For example, if the Pipeline was previously failing but is now successful'
        }
    }
}