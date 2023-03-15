pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'python:3' 
                }
            }
            steps {
                sh 'python -m py_compile hello.py' 
                stash(name: 'compiled-results', includes: '*.py*') 
            }
        }
    }
}