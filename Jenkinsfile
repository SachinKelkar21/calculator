pipeline {
    agent any
    stages {
        stage("compile") {
			steps {
			    sh "mvn springboot:run"
			}	                   
        }
        stage("Unit test") {
			steps {
			    sh "mvn test"
			}	                   
        }
    }
}