pipeline {
    agent any
environment{
    PATH="/opt/apache-maven-3.8.7/bin:$PATH"
}
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
        stage('scm') {
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

