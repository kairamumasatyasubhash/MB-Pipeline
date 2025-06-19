pipeline {
    agent any
    environment {
       DEPLOY_TO = 'production'
    }
    stages {
        satge ('DeployToDev') {
            steps {
                echo "Deploying the environment name"
            }
        }
        stage ('ProdDeploy') {
            when {
                allOf {
                    branch 'production'
                    environment name: 'DEPLOY_TO', value: production
                }
            }
            steps {
                echo "deploying environment production"
            }
        }
    }
}
