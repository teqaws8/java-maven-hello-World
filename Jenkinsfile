pipeline{
    agent any
    environment {
        PATH = "$PATH:/opt/maven/apache-maven-3.8.6/bin"
    }

    //tools {
         //maven 'maven'
         //jdk 'java'
   // }

    stages{
        stage('checkout'){
            steps{
                //checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'github access', url: 'https://github.com/sreenivas449/java-hello-world-with-maven.git']]])
                git 'https://github.com/teqaws8/java-maven-hello-World.git'
            }
        }
        stage('build'){
            steps{
               sh 'mvn package'
            }
        }
    }
}
