pipeline {
    agent any

    triggers {
        githubPush()
    }

    stages {
        stage('Check Changes') {
            steps {
                script {
                    def commitMessage = sh(script: "git log -1 --pretty=%B", returnStdout: true).trim()
                    echo "Latest Commit Message: ${commitMessage}"
                }
            }
        }

        stage('Hello Pipeline') {
            steps {
                script {
                    def istTime = sh(script: "TZ=Asia/Kolkata date '+%d-%m-%Y %I-%M-%S %p'", returnStdout: true).trim()
                    echo 'Hello from Test branch'
                    echo "Build triggered at: ${istTime} IST"
                }
            }
        }
    }
}
