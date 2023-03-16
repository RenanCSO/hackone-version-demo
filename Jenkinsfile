pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent any
            steps {
                sh 'echo comecando a compilacao...'
                sh 'python3 -m py_compile hello.py' 
                stash(name: 'compiled-results', includes: '*.py*') 
            }
        }
    }
}
