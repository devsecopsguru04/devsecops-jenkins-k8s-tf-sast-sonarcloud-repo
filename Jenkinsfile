pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopsatul04 -Dsonar.organization=devsecopsatul04 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b1b953e7be557eacc04a5ac371578f1418d17638'
			}
        } 
  }
}
