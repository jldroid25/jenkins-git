pipeline {
    agent any
    stages {
        
        stage('Build') {
            steps {
                sh 'echo "Jldroid25 - Devops Engineer Integrating Slack Channel "'
                sh '''
                    echo "Jenkins serves with Montreal chattes  !"
                    pwd
                '''
            }
        } 
    }
    
    post {
     always {
       emailext body: "See ${BUILD_URL}", recipientProviders: [requestor()], subject: "Jenkins: ${JOB_NAME}: Build status is ${currentBuild.currentResult}"
     }
   }
    
}
