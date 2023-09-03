pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopsatul -Dsonar.organization=devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=f616b3bf7ad2d501ffd6764effa180a08fbf93a3'
			}
        } 
  }
}
