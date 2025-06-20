pipeline {
    agent any
    parameters {
    choice(name: 'subhash',
    choices: 'yes/no',
    description: "select yes or no"
    )
    choice(name: 'kairam',
    choices: 'yes/no',
    description: "select yes or no"
    )
    choice(name: 'umasatya',
    choices: 'yes/no',
    description: "select yes or no"
    )
    choice(name: 'subbu',
    choices: 'yes/no',
    description: "select yes or no"
    ) 
    stages {
        stage ('UserSelection') {
            steps {
                echo "Please select your name"
            }
        }
    } 
    stage ('UserChoice') {
        steps {
            echo "Please select your choice"
        }
    }
    stage ('UserName') {
        when {
            allOf {
                branch 'subhash'
                environment name: 'USER_NAME', value: 'subbu'
            }
        }
        steps {
            echo "Please select your name"
        }
    }
    stage ('UserChoice') {
        when {
            allOf {
                branch 'kairam'
                environment name: 'USER_NAME', value: 'umasatya'
            }
        }
        when {
            anyOf {
                branch 'kairam'
                environment name: 'USER_NAME', value: 'umasatya'
            }
        }
        steps {
            echo "Please select your choice"
        }
    }
    stage ('UserName') {
        when {
            allOf {
                branch 'subhash'
                environment name: 'USER_NAME', value: 'subbu'
            }
        }
        when {
            anyOf {
                branch 'kairam'
                environment name: 'USER_NAME', value: 'umasatya'
            }
        }
        steps {
            echo "Please select your name"
          }
       }
    }
}
