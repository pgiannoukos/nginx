pipeline {
    agent any
    // agent {
    //     label "main"
    // }
    stages {
        stage('test') {
            steps {
                sh "docker build -t nginx:power ."
            }
        }
    }
}