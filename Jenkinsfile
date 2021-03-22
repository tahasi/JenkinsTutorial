pipeline {
    agent { docker { image 'golang' } }
    
    options {
        skipStagesAfterUnstable()
        buildDiscarder logRotator(
            artifactDaysToKeepStr: '2',
            artifactNumToKeepStr: '2',
            daysToKeepStr: '',
            numToKeepStr: '2')
}

    stages {
        stage('Build') {
            steps {
                sh 'go version'
            }
        }
    }
}

