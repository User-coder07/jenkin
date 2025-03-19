pipeline {
    agent any
    environment{
        JAVA_HOME="C:/Program Files/Java/jdk-21"
        PATH="${JAVA_HOME}\\bin;${env.PATH}"
    }
    stages {
        stage('clone from Github') {
            steps {
                git branch: 'main', url : 'https://github.com/User-coder07/jenkin.git'
            }
        }
        stage('Compile Java Code') {
            steps {
                bat 'javac -d . prashanth/HelloWorld.java'
            }
        }
        stage('Run Java Program') {
            steps {
                bat 'java prashanth.HelloWorld'
            }
        }      
    }
}
