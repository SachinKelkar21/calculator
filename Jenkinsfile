pipeline {
    agent any
    stages {
        stage("compile") {
			steps {
			   def mvnHome = tool name: 'maven-3', type: 'maven'
    		   sh "${mvnHome}/bin/mvn clean package"
			}	                   
        }
        stage("Unit test") {
			steps {
			    sh "mvn test"
			}	                   
        }
    }
}