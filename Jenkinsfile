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
            stage('Slack it'){
            steps {
                slackSend channel: "#jenkinsre", message: "Build Started: ${env.JOB_NAME} ${env.BUILD_NUMBER}"
              }
            }
    
    }
}
