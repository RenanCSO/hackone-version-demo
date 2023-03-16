pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent any
            steps {
                sh 'echo comecando o build...'
                sh 'python3 -m py_compile hello.py' 
                stash(name: 'compiled-results', includes: '*.py*') 
            }
        }
    }
}
