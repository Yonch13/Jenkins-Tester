pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build steps here
            }
        }
    }
    post {
        always {
            echo "Finished running"
        }
        success {
            echo "Success"
        }
    }
}