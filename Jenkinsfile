pipeline {
    agent any
    stages {
        stage("compile") {
			steps {
			    sh "mvn clean package"
			}	                   
        }
        stage("Unit test") {
			steps {
			    sh "mvn test"
			}	                   
        }
    }
}