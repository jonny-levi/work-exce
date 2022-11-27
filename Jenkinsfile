/* groovylint-disable-next-line CompileStatic */
pipeline {
    agent any
    stages {
        stage('fetching') {
            steps {
                sh '''git clone https://github.com/jonny-levi/work-exce.git
                    '''
            }
        }
        stage('building') {
            steps {
                sh 'kubectl create -f work-depolyment.yaml'
            }
        }
        stage('testing') {
            steps {
                sh 'echo testing'
            }
        }
        stage('deploying') {
            steps {
                sh 'echo deploying'
            }
        }
    }
}
