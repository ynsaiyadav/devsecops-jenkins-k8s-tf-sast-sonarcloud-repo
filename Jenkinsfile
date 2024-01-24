pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=aws-sast -Dsonar.organization=aws-sast -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=d60661778e50299081197f4153ede4729ae58bd2'
			}
        } 
  }
}
