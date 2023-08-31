pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=askbuggywebapp -Dsonar.organization=askbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=44531d58ec8e64cd478de77cb0b7633cc0249764'
			}
        } 
  }
}
