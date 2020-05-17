pipeline {
	agent any
	stages {
	  stage('compile') {
	   steps {
		   echo "compiled Successfully";
		}
	}
	  stage('Running') {
	    steps {
		echo "run successful";
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
		   echo ' This will run only if the state of pipeline has changed'
		   echo ' For example, if the pipeline was previousle failed but is now successful'
		}
		
	}
}
