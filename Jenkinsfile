pipeline {
    agent {
        label "jenkins-jenkins-slave"
    }
    stages {
        stage('Initialize') {
            steps {
                container('jnlp') {
                    echo "Testing..."
                    sh "curl google.com"
                }
            }
        }
    }
}