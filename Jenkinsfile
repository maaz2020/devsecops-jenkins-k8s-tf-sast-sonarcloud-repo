pipeline {
  agent any
  tools { 
        maven 'Maven_3_6_3'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=maazsecuritybuggywebbapp -Dsonar.organization=maazsecuritybuggywebbapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=fec880df1b23db04c48e87f82c68f334aa11f675'
			}
        } 
  }
}
