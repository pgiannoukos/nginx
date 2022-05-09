pipeline {
    agent any
    // agent {
    //     label "main"
    // }
    stages {
        stage('test') {
            steps {
                sh "docker build -t nginx:power ."
                sh "docker kill mynginx1 || true"
                sh "docker rm mynginx1 || true"
                sh "docker run --name mynginx1 -p 80:80 -d nginx:power"
            }
        }
    }
}