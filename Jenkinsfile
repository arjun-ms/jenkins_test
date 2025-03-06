pipeline {
    agent any

    triggers {
        githubPush()
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
