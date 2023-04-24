pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=zicobuggy -Dsonar.organization=zicobuggy -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=3c96662fad247ce6484fe9f5891b4b550ac04452'
			}
        } 
  }
}
