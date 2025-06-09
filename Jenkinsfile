pipeline {
    agent any

    stages {
        stage('Build') {
            agent {
                docker {
                    image 'helloworld'
                    reuseNode true
                }
            }
            steps {
                sh '''
                    ls -la
                '''
            }
        }
    }
}
