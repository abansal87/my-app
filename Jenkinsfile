pipeline {
    agent any
    stages {
        stage('clone repo') {
            steps {
                sh "$MAVEN_HOME/mvn clean"
            }
        }
        stage('Test') {
            steps {
                sh "$MAVEN_HOME/mvn test"
            }
        }
        stage('Deploy') {
            steps {
                sh "$MAVEN_HOME/mvn package"
            }
        }
    }
}
