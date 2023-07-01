pipeline {
    agent { 
        node {
            label 'docker-agent-python'
            }
      }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh '''
                ls -ltr
                pwd
                '''
                echo "say you love me..........."
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                python3 hello_jenkins.py
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff.."
                '''
            }
        }
    }
}
