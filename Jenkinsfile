pipeline {
    agent {
        docker { image 'webratio/ant:1.9.6' }
    }
    stages {
        stage('build') {
            steps {
                sh 'ant compile'
            }
        }
        stage('run') {
            steps {
                sh 'ant run'
            }
        }
    }
}
