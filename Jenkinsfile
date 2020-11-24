pipeline {
  agent any
  stages {
      stage('git-chekout') {
      steps {
        git credentialsId: 'e7b17ed4-48c1-413a-b4b1-bc0804b9923f', url: 'https://github.com/prantasaha/jenkins_pipeline_demo.git'
        echo 'pulling codes from git repo'
      }
    }
    stage('code') {
      steps {
        
        echo 'pulling code bat file from git'
        bat 'code.bat'
      }
    }
    stage('build') {
      steps {
        
        echo 'pulling build bat file from git'
        bat 'build.bat'
      }
    }
    stage('test') {
      steps {
        
        echo 'pulling test bat file from git'
        bat 'test.bat'
      }
    }
    stage('deploy') {
      steps {
        echo 'pulling deploy bat file from git'
        bat 'deploy.bat'
      }
    }
  }
}
