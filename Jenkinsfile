pipeline {
stages {
	stage ('Helm Deploy') {
          steps {
            script {
                sh "helm upgrade first --install test-chart --namespace test-namespace"
                }
            }
        }
}
}
