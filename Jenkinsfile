def label = "cloudbees-${UUID.randomUUID().toString()}"
pipeline {	
    agent {
        label 'label'
    }
	stages {

		
    	stage('Build') {				

			steps {
				sh 'echo hello world'
				
			}
		}
	}
}
