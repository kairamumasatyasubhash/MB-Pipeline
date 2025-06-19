pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    satges {
        stage ('ProdDeployToDev') {
            steps {
                echo "Deploying to dev environment"
            }
        }
        stage ('ProdDeploy') {
            when {
                allOf {
                    branch 'production'
                    environment name:'DEPLOY_TO', value :'production'
                }
            }
            steps {
                echo "deploying to production environment"
            }
        }
    }
}
