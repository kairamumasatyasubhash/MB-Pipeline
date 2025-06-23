pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo "Building the application"
            }
        }
    }
    post {
        sucess {
            echo "Build completed successfully!"
        }
        failure {
            echo "Build failed. Please check the logs."
        }
        always {
            echo "This will always run, regardless of the build status."
        }
    }
}
