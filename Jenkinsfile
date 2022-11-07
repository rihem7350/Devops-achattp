pipeline {
   agent any
   stages {
    stage('Git Checkout') {
      steps {
        echo 'pulling...';
         git branch:'rihem',
         url : 'https://github.com/rihem7350/Devops-Achat';
         
         }
        }
    stage('testing maven') {
      steps {
        sh """mvn -version"""
         
         }
        }
    stage('Test mvn') {
            steps {
              sh """ mvn -DskipTests clean package """
                sh """ mvn install """;
                sh """ mvn test """;
            }
        }
 

       }
      }
