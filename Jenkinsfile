pipeline {
  agent any
  stages {
    steps {
      load "$JENKINS_HOME/workspace/WEB-CI-CD/dev/env.sh"
      sh "sshpass -p ${env.TARGET_PASSWD} ssh -o StrictHostKeyChecking=no ${env.TARGET_HOST}"
      sh "sshpass -p ${env.TARGET_PASSWD} ssh -o StrictHostKeyChecking=no ${env.TARGET_HOST} 'hostname'"
      sh "sshpass -p ${env.TARGET_PASSWD} ssh -t -o StrictHostKeyChecking=no ${env.TARGET_HOST} 'mkdir -p ${env.DIR}'"
      sh "sshpass -p ${env.TARGET_PASSWD} ssh -t -o StrictHostKeyChecking=no ${env.TARGET_HOST} 'cd ${env.DIR};rm -rf ${env.DIR}'"
      
      sh "sshpass -p ${env.TARGET_PASSWD} ssh -t -o StrictHostKeyChecking=no ${env.TARGET_HOST} 'git clone  ****** echo "${env.TARGET_HOST}"
      echo "${env.BUILD_DISPLAY_NAME}"
      echo "$JENKINS_HOME"
     
     }
}
      