pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Hi') {
            steps {
                echo 'How are you'
            }
        }
      stage('SCM') {
            steps {
                git 'https://github.com/manju47/hello-world.git'
            }
        }
         stage('build') {
            steps {
                sh "mvn package"
            }
        }
    }
}

