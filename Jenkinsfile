pipeline {
agent {
node {
label 'roboshop'
}
}

```
environment {
    COURSE = "Jenkins"
}

stages {
    stage('Build') {
        steps {
            sh '''
                echo "Building"
            '''
        }
    }

    stage('Test') {
        steps {
            sh '''
                echo "Testing"
                echo $COURSE
            '''
        }
    }

    stage('Deploy') {
        steps {
            sh '''
                echo "Deploying"
            '''
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
```

}
