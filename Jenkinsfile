pipeline {
    agent any

    stages {
        stage("Code") {
            steps {
                script {
                    // Determine the branch name dynamically
                    def branchName = sh(script: 'git rev-parse --abbrev-ref HEAD', returnStdout: true).trim()
                    echo "Current branch: ${branchName}"
                    
                    git url: "https://github.com/Anurag-Evervent/nodemysql.git", branch: branchName
                }
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
