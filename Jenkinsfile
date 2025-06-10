pipeline {
    agent {
        docker { image 'node:24-alpine' }
    }
    stages {
        stage('Clone the repos') {
            steps {
                echo 'Cloning frontend repository'
                git branch: 'main',
                    url: 'https://github.com/w-burgis/devops-er-frontend.git'
                echo 'Was frontend cloned?'
                sh 'ls -a'
            }
        }
    }
}
