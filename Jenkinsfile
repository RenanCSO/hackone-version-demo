pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent any
            steps {
                sh 'python -m py_compile hello.py' 
                stash(name: 'compiled-results', includes: '*.py*') 
            }
        }
    }
}