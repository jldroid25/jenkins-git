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
       slackSend  channel: "jenkinsre",  message: "${env.BUILD_URL} ${env.JOB_NAME} ${env.currentBuild.currentResult}"
     }
   }
    
}
