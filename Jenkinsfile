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
       slackSend message: "See ${BUILD_URL}", channel: "Jenkinsre: ${JOB_NAME}: Build status is ${currentBuild.currentResult}"
     }
   }
    
}
