pipeline {
    agent any
    environment {
       DEPLOY_TO = 'production'
    }
    stages {
        satge ('DeployToDev') {
        }
        stage ('ProdDeploy') {
            when {
                allOf {
                    branch 'production'
                    environment name: 'EPLOY_TO', value: production
                }
            }
            steps {
                echo "deploying environment production"
            }
        }
    }
}
