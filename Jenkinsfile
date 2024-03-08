pipeline {
  agent any

  tools {
    jdk "jdk17"
    maven "M3"
  }
  
    stages {
      stage('Git clone'){
        steps {
            echo 'Git clone'
            git url: 'https://github.com/keg1213/spring-petclinic.git',
              branch: 'efficient-webjars'
        }
      }
    }
    post {
      success {
        echo 'Git clone Success!!'
      }
      failure {
        echo 'Git clone Fail'
      }
  }
}
