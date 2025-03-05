pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello from Test branch'
                echo "Build triggered at: ${new Date()}"
            }
        }
    }
}
