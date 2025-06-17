pipeline {
    agent {
        docker { image 'node:22.16.0-alpine3.22' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --eval "console.log(process.arch,process.platform)"'
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
        failure {
            echo "Failed"
        }
    }
}