pipeline {
    agent any
    environment {
       DEPLOY_TO = 'production'
    }
    stages {
        stage ('ProdDeployToDev') {
         }
            stage ('DeplotToDev') {
                when {
                    allOf {
                 barnch 'production'
                 environment name:'DEPLOY_TO',  value:'production'                  }
                }
            }
            steps {
                echo "deploying the production environment"
            }
         }
    }
