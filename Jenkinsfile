pipeline {
    agent { node { label 'workstation' } }

    environment {
      ssh = credentials('ssh')
    }
    stages {
        stage('Hello-1') {
            steps {
                echo 'Hello World-1'
                echo 'env'
            }
        }
    }
    post{
    always{
      sh "echo post"
    }
    }
}