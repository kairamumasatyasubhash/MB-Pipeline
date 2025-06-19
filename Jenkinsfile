pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('ProdDeploy') {
            when {
                not {
                    equals expected :"Prod", actual :"${DEPLOY_TO}"
                }
            }
            steps {
                echo "Deploy production"
            }
        }
    }
}
