pipeline {
    agent any
    environment {
       Deploy_To = 'subhash'
    }
    stages {
        stage ('Build') {
            when {
                environment name: Deploy_To, value : 'subhash'
            }
            steps {
            echo "print the subhash"
             }
          }
       }
    }
