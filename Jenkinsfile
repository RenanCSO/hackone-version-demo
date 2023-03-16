pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent any
            steps {
                sh 'echo começando o build...'
                sh 'python3 -m py_compile hello.py' 
                stash(name: 'compiled-results', includes: '*.py*') 
            }
        }
    }
}
