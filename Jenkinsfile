pipeline {
    agent { node { label 'workstation' } }

    stages {
        stage('Hello-1') {
            steps {
                echo 'Hello World-1'
            }
        }
    }
    post{
    always{
      sh "echo post"
    }
    }
}