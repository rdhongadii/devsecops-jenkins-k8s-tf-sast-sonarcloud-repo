pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=appsecc -Dsonar.organization=appsecc -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=cec9edf6effe8a78f05cf2822d1431e67f23efda'
			}
        } 
  }
}
