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
        
        stage('Pipeline Slack Info') {
            steps {
                slackSend failOnError: true, channel: "#jenkinsre", message: " Successful Build: for  (<${env.BUILD_URL}open>) ${env.JOB_NAME} ${env.BUILD_NUMBER}"
                
            }
        } 
       
        
   }
    
}
