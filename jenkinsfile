pipeline {
   agent any
   stages {
       stage('example') {
           steps {
               script {
                   wrap([$class: 'BuildUser']) {
                       echo "BUILD_USER=${BUILD_USER}"
                       echo "BUILD_USER_FIRST_NAME=${BUILD_USER_FIRST_NAME}"
                       echo "BUILD_USER_ID=${BUILD_USER_ID}"
                       echo "BUILD_USER_EMAIL=${BUILD_USER_EMAIL}"
                       echo "---"
                       echo "env.BUILD_USER=${env.BUILD_USER}"
                       echo "env.BUILD_USER_FIRST_NAME=${env.BUILD_USER_FIRST_NAME}"
                       echo "env.BUILD_USER_ID=${env.BUILD_USER_ID}"
                       echo "env.BUILD_USER_EMAIL=${env.BUILD_USER_EMAIL}"
                       echo "env.JENKINS_HOME=${JENKINS_HOME}"
                   }
               }
           }
       }
   }
}
 
