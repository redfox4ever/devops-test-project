pipeline {
    agent any

    tools {
        maven "M2_HOME"
    }

    stages {
        stage('GIT') {
            steps {
                git branch: 'main',
                url: 'https://github.com/redfox4ever/devops-test-project',
                credentialsId: 'jenkins-exam-github-pat'

            }
        }
        stage('MAVEN'){
            steps {
                sh "mvn -version"
            }
        }
    }
}
