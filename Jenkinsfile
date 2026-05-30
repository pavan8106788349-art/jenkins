pipeline {
    agent {
        node {
            label 'roboshop'
        }
    }

    stages {
        stage('Build') {
            steps {
                script {
                    sh '''
                        echo "Building"
                    '''
                }
            }
        }
        environment{
            COURSE = "Jenkins"
        }
        stage('Test') {
            steps {
                script {
                    sh '''
                        echo "Testing"
                        echo $COURSE
                    '''
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    sh '''
                        echo "Deploying"
                    '''
                }
            }
        }
    }

    post {
        always {
            echo 'I will always say Hello again!'
        }
        success {
            echo "pipeline success"
        }
        failure {
            echo "pipeline failure"
        }
    }
}


