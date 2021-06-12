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
                buildingTag()
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
