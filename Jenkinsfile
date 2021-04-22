pipeline {
    agent any
    stages {
        stage('check service') {
            steps {
                echo "Hello Ist stage"
                sh service httpd status
            }
        }
        stage('install') {
            steps {
                echo "Hello 2nd stage"
                sh yum install httpd -y
            }
        }
        stage('start service') {
            steps {
                echo "Hello 3rd stage"
                sh systemctl start httpd
            }
        }
        stage('enable service') {
            steps {
                echo "Hello final stage"
                sh systemctl enable httpd
                
            }
        }
    }
}
