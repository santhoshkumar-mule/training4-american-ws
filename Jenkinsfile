pipeline {
    agent any
    stages { 
        stage('Example') {
            steps {
            deleteDir()
            checkout scm
                echo 'Hello World'
                
            }
        }
        stage('build the code'){
             steps              {
               echo 'build checking'
               bat 'mvn  clean package -DskipTests'
                                  }
                       }
         stage('run munits'){
             steps              {
               echo 'build checking'
               bat 'mvn test'
                                  }
                       }
              }
}

