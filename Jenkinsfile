pipeline {
    agent any            
    tools {             
        jdk "jdk21.0.8"
    }
    stages {             
        stage('Checkout code') {
            steps {
                git branch: 'master', url: 'https://github.com/Mariem-9/DEVOPS_TPs.git'
            }
        }
        stage('Compile code') {
            steps {
                sh 'javac src/application/test.java'
            }
        }
        stage('EXecute code') {
            steps {
                sh 'java -cp src application.test'
            }
        }
    }

}

