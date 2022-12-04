pipeline {
    agent {label 'kubemaster1'}
    stages {
        stage('fetching') {
            steps {
                sh '''
                rm -rf work-exce
                git clone https://github.com/jonny-levi/work-exce.git
                    '''
            }
        }
        stage('building') {
            steps {
                sh ''' cd webapp-1
                kubectl delete -f .
                kubectl create -f .'''
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