pipeline {
    agent { node { label 'workstation' } }



  environment {
    SSH = credentials('SSH')
  }
 options {
  ansiColor('xterm')
  }

 triggers { pollSCM('h/2 * * * *') }

 parameters {
 string(name: 'app_input', defaultValue: '', description: 'just input')
}
    stages {
        stage('Hello-1') {
            steps {
                echo 'Hello World-1'
                sh 'env'
            }
        }
    }
    post{
    always{
      sh "echo post"
    }
    }
}