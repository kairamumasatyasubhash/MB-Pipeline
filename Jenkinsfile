pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo "bulding the code"
            }
        }
        stage ('parallelscaning') {
            parallel {
                stage ('code quality') {
                    steps {
                        echo "checking the code quality of the machine"
                        sleep 10
                    }
                }
                stage ('securesystem') {
                    steps {
                        echo "secureing the system"
                        sleep 10 
                    }
                }
                stage ('protect the system'){
                    steps {
                        echo "the system will be protected"
                        sleep 10
                     }
                 }
              }
           }
        }
     }
