pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh "chmod +x gradlew"
                sh "echo build"
                sh "./gradlew build"
            }
        }
	stage('deploy to tomcat'){
	    steps{
	         sh "cp ./build/libs/wherebackend.war /opt/tomcat/webapps"

	    }
	}

    }
}
