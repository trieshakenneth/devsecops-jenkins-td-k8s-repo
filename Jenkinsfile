pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sampleapp-devsecops_sampleproject -Dsonar.organization=sampleapp-devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=ff7717029cda7498a09f252f9f5a3392f859ea22'
			}
        } 
  }
}
