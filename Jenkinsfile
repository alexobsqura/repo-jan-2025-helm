pipeline {
	agent any
	stages {
		stage ('Helm Deploy') {
	          steps {
	            script {
			sh 'aws ecr get-login-password --region eu-north-1 | docker login --username AWS --password-stdin 605134450606.dkr.ecr.eu-north-1.amazonaws.com/alexobsqura/node-app-repo'
	                sh "helm upgrade first --install test-chart --namespace test-namespace"
	                }
	            }
	        }
	}
}
