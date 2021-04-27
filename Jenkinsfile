pipeline {
    agent any
    stages { 
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
    }
}

stage("build the code"){
   echo 'build checking'
   sh 'mvn clean install'
}