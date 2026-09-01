pipeline {
    agent {
        node
        {
            label 'AGENT-1'
        }
    }
    stages {
        stage('Build') {
            steps {
                echo "building"
            }
        }
        stage('Test') {
            steps {
                echo "testing"
            }
        }
        stage('Deploy') {
            steps {
                echo "deployimg"
            }
        }

        post {
          always {
            echo 'i will always say hello again'
            cleanWs()
        }
        success {
            echo 'i will if success'
            
        }
        failure {
            echo 'i will run if failure'
        }
    }
}
