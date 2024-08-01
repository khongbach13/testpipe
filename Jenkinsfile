pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', 
                    url: 'git@github.com:khongbach13/testpipe.git'
            }
        }
    }
}
