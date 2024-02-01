pipeline {
  agent any
	tools { 
        maven 'Maven_3_8_6'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp -Dsonar.organization=asgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=e312fef18672b10d04040b5677f418c412ea188f'
			}
        } 
  }
}

