pipeline {
   agent any

   stages {
      stage('checkout') {
         steps {
            echo 'Cloning the project'
          checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'dd5e5314-7300-4266-99be-6d49a265413d', url: 'https://github.com/ghantauttej/MyCab.git']]])
         }
      }
      stage('Build') {
         steps {
            echo 'Build the project'
         }
      }
       stage('Test') {
         steps {
            echo 'Test has run successfully'
         }
      }  
      stage('QA Deploy') {
         steps {
            echo 'QA deploy the project'
         }
      }
 stage('Prod Deploy') {
         steps {
            echo 'Prod Deploy the project' 
	  }
	 }
   }
}
