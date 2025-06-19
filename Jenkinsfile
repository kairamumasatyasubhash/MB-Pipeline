pipeline {
    agent any
    environment {
        user-name = 'subhash'
    }
    stages {
        stage ('DEPLOYING') {
            when {
                environment name: user-name, value : 'subhash'
            }
            echo "print the value"
        }
    }
}
