pipeline {
    agent any

    triggers {
        githubPush()
    }

    stages {
        stage('Pull Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/mukundDeo9325/task_red.git'
            }
        }
    }

    post {
        success {
            echo "✅ Code pulled successfully"
        }
        failure {
            echo "❌ Pull failed"
        }
    }
}
