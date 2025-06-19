pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('ProdDeploy') {
        }
     }
         stage ('ProdDeploy') {
            when {
                allOf {
                    environment name:'DEPLOY_TO', value :'production'
            }
            steps {
                echo "deploying to production environment"
            }
        }
    }
}
