pipeline {
    agent any
    environment {
       DEPLOY_TO = 'production'
    }
    stages {
        stage ('DeployToDev') {
         }
            stage ('ProdDeploy') {
                when {
                    allOf {
                 branch 'production'
                 environment name:'DEPLOY_TO',  value:'production'                  }
                }
            }
            steps {
                echo "deploying the production environment"
            }
         }
    }
