pipelines {
    agent any
    environment {
        course = "docker and k8"
        name ="subhash"
     }
     stages {
        stage ('build') {
            cloud = "GCP"
            steps {
                echo "welcome ${name}"
                echo "you are selected for this ${course}"
                echo "you are selected for ${cloud}"
            }
        }
     }
}
