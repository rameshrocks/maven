node
         {
         stage('SCM'){
                   checkout([$class: 'GitSCM', 
                   branches: [[name: '*/master']], 
                   doGenerateSubmoduleConfigurations: false, 
                   extensions: [],
                   submoduleCfg: [],
                   userRemoteConfigs: [[url: 'https://github.com/rameshrocks/maven.git']]])
               }
               stage('build'){
                   sh"""
                      mvn clean package -DskipTests=true
                      ls -lrt
                      ls -lrt ${workspace}/target
                      cd ${workspace}/target
                      zip -r ${workspace}/deploy.zip *.jar
                      """
               }
               cleanWs()
          }  
     
