pipeline{
    agent any
    stages{
        stage('Build') {
            steps {
                bat 'docker build -t react-external .'
            }
        }
        stage('Run') {
            steps {
                bat 'docker run -d -p 3000:3000 react-external'
            }
        }
    }
}