pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building.. ${TAG_NAME}'
            }
        }
        stage('Test') {
            when {
                buildTags()
            }
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
