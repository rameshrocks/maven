node
     
     {
         stage('SCM'){
        
                   checkout([$class: 'GitSCM', 
                   branches: [[name: '$BRANCH']], 
                   doGenerateSubmoduleConfigurations: false, 
                   extensions: [],
                   submoduleCfg: [],
                   userRemoteConfigs: [[url: 'https://github.com/rameshrocks/maven.git']]])
               }
     }  
