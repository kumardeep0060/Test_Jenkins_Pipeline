pipeline {
    agent any
    stages {
        stage('check service') {
            steps {
                echo "Hello Ist stage"
                sh 'rm -rf test'
            }
        }
        stage('install') {
            steps {
                echo "Hello 2nd stage"
                //yum install httpd -y
            }
        }
        stage('start service') {
            steps {
                echo "Hello 3rd stage"
                //systemctl start httpd
            }
        }
        stage('enable service') {
            steps {
                echo "Hello final stage"
                //systemctl enable httpd
                //echo "Hello from $(hostname -f)" > /var/www/html/index.html
            }
        }
    }
}
