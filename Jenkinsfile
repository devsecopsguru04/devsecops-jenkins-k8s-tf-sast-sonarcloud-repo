pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopsatul -Dsonar.organization=devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=c1cbe497fdb61766447b7b73755862598f5534e1'
			}
        } 
  }
}
