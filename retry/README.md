pipeline {
    agent any
    stages {
        stage ('Timeout-MP') {
            steps {
                retry(3){
                    sh "echo hello world"
                }

            }
        }
    }
}
