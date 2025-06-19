pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo "bulding the code"
            }
        }
        satge ('parallelscaning') {
            parallel {
                stage ('code quality') {
                    steps {
                        echo "checking the code quality of the machine"
                    }
                }
                stage ('securesystem') {
                    steps {
                        echo "secureing the system"
                    }
                }
            }
        }
    }
}
