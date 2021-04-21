pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
               sh "rm -rf TicketBookingServiceJunitTesting"
                sh "git clone https://github.com/kumardeep0060/Test_Jenkins_Pipeline.git"
                sh "mvn clean -f TicketBookingServiceJunitTesting"
            }
        }
        stage('install') {
            steps {
                sh "mvn install -f TicketBookingServiceJunitTesting"
            }
        }
        stage('test') {
            steps {
                sh "mvn test -f TicketBookingServiceJunitTesting"
            }
        }
        stage('package') {
            steps {
                sh "mvn package -f TicketBookingServiceJunitTesting"
            }
        }
    }
}
