pipeline {
    agent { docker 'node:6.3' }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
            }
        }
        stage('deploy') {
            agent { docker 'maven:3.3.3' }
                steps {
                    sh 'mvn --version'
                }
        }
    }
  environment {
    foo = 'bar'
  }
}
