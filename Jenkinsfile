//Srcipted Style
//node {
 //  stage('Checkout'){
  //    echo "Inside Stage Checkout"
   //   checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'GIT_CREDS', url: 'https://github.com/jagdevops19/jenkinsscripts.git']]])
    // }
  // stage('running script'){
   //    echo "inside running script"
    //   sh label: '', script: '''chmod +x print.sh
//./print.sh'''
 //  }
//}

//Declrative Way Style
pipeline {
     agent any
        stages {   
     stage ('Checkout2'){
     steps {
     sh 'echo hellohello'

      echo "Inside Stage Checkout2"
      checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions:[], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'GIT_CREDS', url: 'https://github.com/jagdevops19/jenkinsscripts.git']]])
       }
      }
   stage('running script'){
      steps{
       echo "inside running script"
       sh label: '', script: '''chmod +x print.sh
./print.sh'''
     }
    }
}
}

