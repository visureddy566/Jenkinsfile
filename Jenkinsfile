pipeline {
    agent any 

    environmnt{
        PATH = "/opt/apache-maven-3.6.3/bin:$PATH"
    }
    stages {
        stage('clone code') {
            steps {
                git 'https://github.com/visureddy566/helloworld-java-maven.git'
            }
        }
        stages ("Maven Build"){
            steps{
                sh "mvn clean package"
            }
        }
    }
}
