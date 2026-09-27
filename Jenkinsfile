pipeline {
    agent any

    environment {
        KUBECONFIG = '/var/jenkins_home/.kube/config'
    }

    stages {
        stage('Deploy') {
            steps {
                sh 'helm upgrade --install demo microservices/msvc-chart --namespace demo'
            }
        }
    }
}
