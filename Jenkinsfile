pipeline {
    agent {
        label "jenkins-jenkins-slave"
    }

    options {
        buildDiscarder(logRotator(numToKeepStr: '30'))
    }

    stages {
        stage('Initialize') {
            steps {
                container('jnlp') {
                echo "Testing..."
                //   script {
                //     def response = httpRequest(url:'http://grove-gateway-webhook:12000/',contentType: 'APPLICATION_JSON',httpMode: 'POST', requestBody: '{"companyId":"kms","version": "2.7.7","targetEnvironment": "dev","tenantId": "5bfe11fe183977463bbf63dc"}')
                //   }
                sh "curl google.com"
                }
            }
        }
    }
}