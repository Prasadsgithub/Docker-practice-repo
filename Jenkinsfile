pipeline {
    agent { label 'DOCKER'}
    options {
        timeout(time: 1, unit: 'HOURS')
    }
    triggers {
        pollSCM('* * * * *')
    }
    stages {
        stage('testing-docker') {
            steps {
                sh 'docker info'
                  
            }
        }
       
    }
}