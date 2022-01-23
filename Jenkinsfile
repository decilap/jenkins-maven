
peline {
    agent any
    stages {
        stage('clone') {
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/decilap/test-java.git"
            }
        }
        stage('Build') {
            steps {
                sh "cd  test-java && javac App.java"
                sh "java -version"
            }
        }
       stage('run') {
            steps {
                sh "cd  test-java && java FirstApp"
            }
        }
     
    }
}}
