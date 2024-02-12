pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
             
                git 'https://github.com/Anurag-Evervent/nodemysql.git'
            }
        }
        }
    }

    post {
        success {
            // Add success post-build actions here if needed
        }
        failure {
            // Add failure post-build actions here if needed
        }
    }
}
