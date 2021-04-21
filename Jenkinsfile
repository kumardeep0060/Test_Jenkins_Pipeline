pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
                echo "Hello Ist stage"
            }
        }
        stage('install') {
            steps {
                echo "Hello 2nd stage"
            }
        }
        stage('test') {
            steps {
                echo "Hello 3rd stage"
            }
        }
        stage('package') {
            steps {
                echo "Hello final stage"
            }
        }
    }
}
