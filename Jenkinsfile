pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                sh 'helm upgrade --install demo microservices/msvc-chart --namespace demo'
            }
        }
    }
}
