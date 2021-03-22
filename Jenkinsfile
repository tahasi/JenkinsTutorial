pipeline {
    agent { docker { image 'golang' } }
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') {
            steps {
                sh 'go version'
            }
        }
    }
}

