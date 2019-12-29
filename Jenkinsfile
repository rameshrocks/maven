#!groovy
pipeline{
  stages{
      stage("SCM){
           steps{
               script{
                   STAGE_NAME="SCM"
                   gitinfo = checkout scm
                   echo "$gitinfo.GIT_COMMIT"
               }
           }
      }
  }  
}
