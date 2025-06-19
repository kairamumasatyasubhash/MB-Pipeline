pipeline {
    agent any
    environment {
       USER_NAME = 'subhash'
    }
    stages {
        stage ('DEPLOYING') {
            when {
                environment name: USER_NAME, value : 'subhash'
            }
            echo "print the value"
        }
    }
}
