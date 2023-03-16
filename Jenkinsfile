pipeline {
  agent any
  tools { 
        maven '3.5.0'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sadigovanar -Dsonar.organization=sadigovanar -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=382c746aa949b768df5ab3edce6e13c817d860ad'
			}
        } 
  }
}
