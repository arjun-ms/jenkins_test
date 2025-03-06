pipeline {
    agent any

    triggers {
        pollSCM('* * * * *') // Checks for changes in Git every minute
    }

    stages {
        stage('Hello  Piepline') {
            steps {
                echo 'Hello from Test branch'
                echo "Build triggered at: ${new Date()}"
            }
        }
    }
}
