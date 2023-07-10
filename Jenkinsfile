pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'Building happens'
            }
        }
    }

    post {
        success {
            emailext attachLog: true, body: 'send the email', subject: 'email sent', to: 'utkarshpathak562@gmail.com'
        }
    }
}

