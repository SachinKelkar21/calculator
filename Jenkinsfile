pipeline {
    agent any
    tools { 
        maven 'Maven 3.6.1' 
        jdk 'jdk8' 
    }
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
            }
        }

        stage ('Build') {
            steps {
                echo 'This is a minimal pipeline.'
            }
        }
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