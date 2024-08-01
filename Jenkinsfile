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
            sh 'curl -iX GET "https://api.telegram.org/7138980867:AAFSCc-O_l1owbq6mdQBb0J6W18dMvYS0l0/sendMessage?chat_id=-4215079471&parse_mode=HTML&text=<b>Project</b> : jenkinsnew <b>Branch</b>: master <b>Build </b> : SUCCESS"'
        }
    
        failure{
            sh 'curl -iX GET "https://api.telegram.org/7138980867:AAFSCc-O_l1owbq6mdQBb0J6W18dMvYS0l0/sendMessage?chat_id=-4215079471&parse_mode=HTML&text=<b>Project</b> : jenkinsnew <b>Branch</b>: master <b>Build </b> : FAILURE"'
        }
        
    }
}
