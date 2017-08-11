pipeline {
agent any
    parameters {
		booleanParam(
            name: 'test', 
            defaultValue: false , 
            description: 'Test')
		}	
   stages {
		stage('Test') {
			if(params.test){
				build(
					job: 'Jenkinsfile.test',
				)
			}
		}
    }
}

