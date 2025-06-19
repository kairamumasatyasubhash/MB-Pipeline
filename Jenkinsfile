pipeline {
    agent any
    environment {
       DEPLOY_TO = 'production'
    }
    stages {
        stage ('ProdDeployToDev') {
            steps {
                 echo "deploying the production"
            }
         }
         stages {
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
}
