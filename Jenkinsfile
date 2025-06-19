pipeline{
    agent any 
    environment {
        USER_NAME = 'subhash'
    }
    stages {
        stage ('UserIsSubhash') {
            steps {
                echo "my name is subhash"
            }
        }
        stage ('SubhashKairam') {
            when {
                anyOf{
                    branch 'subhash'
                    environment name:'USER_NAME', value:'subbu'
                }
            }
            steps {
                echo "kairam uma satya subhash"
            }
        }
    } 
}
