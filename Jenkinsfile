pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=pavithra-devops_devsecops -Dsonar.organization=pavithra-devops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=768ee2edc76f25fa11240f65b225527718b02f30'
			}
        } 
  }
}
