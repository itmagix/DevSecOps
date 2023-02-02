pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=hackwerk -Dsonar.organization=hackwerk -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=979bb17e1a03c1dc2c731bbcec3c9c93835c3bb5'
			}
        } 
  }
}
