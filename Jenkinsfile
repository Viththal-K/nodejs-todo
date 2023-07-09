pipeline {
    agent any

    stages {
        stage('Git Clone') {
            steps {
                echo "Cloning the code"
                git 'https://github.com/Viththal-K/nodejs-todo.git'
            }
        }
        stage('Build') {
            steps {
                echo "Installing npm"
                sh 'npm install'
            }
        }
        stage('Run') {
            steps {
                echo "Running the application"
                sh 'nohup node index.js'
            }
        }
    }
}
