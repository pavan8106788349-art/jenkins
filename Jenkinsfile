pipeline {
    agent {
        node {
            label 'ROBOSHOP'
        }
    }
    environment {
        COURSE = "Jenkins"
    }
    stages {
        stage('Build') { 
            steps {
                script{
                    sh '''
                       echo "Building"
                       echo $COURSE
                    '''
                }
            }
        }
        stage('Test') { 
            steps {
                script{
                    sh '''
                      echo "Testing"
                    '''
                }
            }
        }
        stage('Deploy') { 
            steps {
                script{
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
    
