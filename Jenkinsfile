pipeline {
    agent any

    stages {
        stage('Prod') {
            when {
                anyOf {
                    environment name: 'GIT_BRANCH', value: 'origin/main'
                }
            }
            steps {
                echo 'Building..'
            }
        }

    }
}
