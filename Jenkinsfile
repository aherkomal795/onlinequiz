pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/aherkomal795/onlinequiz.git'
            }
        }

        stage('Compile') {
            steps {
                sh 'javac OnlineQuizApplication.java'
            }
        }

        stage('Run Program') {
            steps {
                sh 'java onlinequizapplication.OnlineQuizApplication'
            }
        }
    }
}
