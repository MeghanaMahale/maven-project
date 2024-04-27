pipeline {
    agent any

    tools {
        maven "default"
    }

    stages {
        stage('Build') {
            agent any
		
	    steps
	    {
		echo "Build stage"
               
                git branch: 'master', url: 'https://github.com/MeghanaMahale/maven-project.git'

                sh "mvn -Dmaven.test.failure.ignore=true clean test package install"
             }
        }
    }
}
