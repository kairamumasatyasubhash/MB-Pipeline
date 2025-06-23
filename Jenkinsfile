pipeline {
    agent any
    parameters {
        string(name: 'user-name', defaultValue: 'subhash', description: 'Enter your name')
    }
        stages {
        stage ('UserInput') {
            steps {
                script {
                    def userName = params['user-name']
                    echo "User name is: ${userName}"
                }
            }
        }
    }
}
