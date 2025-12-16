pipeline {
    agent any
    environment{
        PATH = "/opt/maven/bin:$PATH"
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/pradeepreddy3097/sparkjava-war-example.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
