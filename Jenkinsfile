#!groovy
pipeline{
  stages{
      stage("SCM){
           steps{
               script{
                   Scheckout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/rameshrocks/maven.git']]])
               }
           }
      }
  }  
}
