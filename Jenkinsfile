pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                bat 'mvn -Dmaven.test.failure.ignore=true clean package -s C:/Java/apache-maven-3.6.3/conf/settings.xml'
            }
        }

        stage('test') {
            steps {
                bat 'mvn test -s C:/Java/apache-maven-3.6.3/conf/settings.xml'
            }
        }
    }
}
