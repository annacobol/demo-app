pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'docker build -t my-demo-app .'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'docker run --rm my-demo-app node -e "console.log(\'Test passed\')"'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Здесь можно добавить команды для деплоя, например, запуск контейнера
            }
        }
    }
}
