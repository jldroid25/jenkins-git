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
        exit 1
        
        stage('Pipeline Slack Info') {
            steps {
                slackSend failOnError: no, channel: "#jenkinsre", message: " Successful Build for:   ${env.JOB_NAME}  ${env.BUILD_NUMBER}  (<${env.BUILD_URL}open>) "
                
            }
        } 
        
         stage('Pipeline Slack Failure MSG') {
            steps {
                slackSend failOnError: true,  message: " Pipeline/Job Failed see:   ${env.JOB_NAME}  ${env.BUILD_NUMBER}  (<${env.BUILD_URL}open>) "
                
            }
        } 
       
        
   }
    
}
