pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('ProdDeploy') {
        }
        steps {
        echo "deploying to production environment"     
     }
         stage ('ProdDeploy') {
            when {
                anyOf {
                    environment name:'DEPLOY_TO', value :'production'
            }
            steps {
                echo "deploying to production environment"
             }
          }
      }
   }
}
