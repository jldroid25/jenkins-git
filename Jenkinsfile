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
            stage('Slack it'){
            steps {
                slackSend channel: '#jenkisre', 
                          message: 'Hello, did you see MTL?'
              }
            }
        }
    }
}
