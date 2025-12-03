pipeline {
    agent any


   tools {
       maven 'maven3'
   }

  triggers {
    githubPush()
  }
  
    stages {
        stage('git checkout') {
            steps {
                git 'https://github.com/Msocial123/maven-web-application.git'
            }
        }
        
                stage ('maven build war file'){
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
