pipeline {
    agent any
    environment {
       USER_NAME = 'subhash'
    }
    stages {
        stage ('Deploy') {
            when {
                environment name: USER_NAME, value : 'subhash'
            }
            echo "print the value"
        }
    }
}
