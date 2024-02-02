pipeline {
  agent any
	tools { 
        maven 'Maven_3_6_3'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sonar08 -Dsonar.organization=sonar08 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=fab8caf2ae55cefdab420c42492b88c56e4ed4f3'
			}
        } 
  }
}

