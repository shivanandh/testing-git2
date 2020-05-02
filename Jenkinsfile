pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install petclinic-app testing-git  --set image.repository=registry.hub.docker.com/shivanandh/testing-git --set image.tag=2'
              			
            }           
        }
    }
}
