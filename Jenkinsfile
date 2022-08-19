pipeline {
    agent any

    stages {
        stage('Build') {
		    when {
                anyOf {
                    environment name: 'GIT_BRANCH', value: 'origin/ups_eks'
                    environment name: 'GIT_BRANCH', value: 'origin/development'
                    environment name: 'GIT_BRANCH', value: 'origin/master'
                }
            }
            steps {
                echo 'Building..'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        
        stage('Test_2') {
            steps {
                echo 'Testing.22.'
            }
        }        
        
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
