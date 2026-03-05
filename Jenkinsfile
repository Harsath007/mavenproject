pipeline {
    

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/Harsath007/mavenproject.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }

        stage('Package') {
            steps {
                bat 'mvn clean package'
            }
        }
    }
}
