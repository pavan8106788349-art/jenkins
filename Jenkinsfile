pipeline {
    agent {
        node {
            label 'roboshop
            }
        }
    }        

    stages {
        stage('Build') {
            steps {
                script{
                    sh """
                        echo "Building"
                    sh """    
                }
            }
        }
        stage('Test') {
            steps {
                script{
                    sh """
                      echo "Testing"
                      exit 1
                    sh """  
                }
            }
        }
        stage('Deploy') {
            steps {
                script{
                      sh """
                        echo "Deploying"
                      sh """  
                }
            }
        }
    }
}

  // post build
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