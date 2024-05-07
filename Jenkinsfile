pipeline {
    agent any
    stages {
       stage('build') {
           steps {
             echo " this is build"
            }
        }
       stage('test parallel') {
        parallel {
           stage('test on chrome') {
             steps {
               echo " this is test on chrome browser"
             }
          }
         stage('test on opera') {
             steps {
               echo " this is test on opera browser"
             }
          }
        }
      }
      stage('deploy') {
           steps {
             echo " this is deploy"
            }
        }
}
}


