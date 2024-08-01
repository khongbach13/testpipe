pipeline {
    
    agent any
    stages {
        stage('Build') {
            steps{
                git url: 'https://github.com/khongbach13/testpipe/'
            }
            
        }
    }
    post{
        success{
            sh 'curl -s -X POST "https://api.telegram.org/bot7138980867:AAFSCc-O_l1owbq6mdQBb0J6W18dMvYS0l0/sendMessage" -d "chat_id=-4215079471&text=Hello20from%20Bot!"'
        }
    
        failure{
            sh 'curl -s -X POST "https://api.telegram.org/bot7138980867:AAFSCc-O_l1owbq6mdQBb0J6W18dMvYS0l0/sendMessage" -d "chat_id=-4215079471&text=Hello20from%20Bot!"'
        }
        
    }
}
