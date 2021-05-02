pipeline {
    agent any
    stages { 
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
        stage('build the code'){
             steps              {
               echo 'build checking'
               sh 'mvn  clean package -DskipTests'
                                  }
                       }
              }
}

