pipeline{
	agent any
    parameters {
		booleanParam(
            name: 'test', 
            defaultValue: false , 
            description: 'Test')
		}	
   stages {
		stage('Test') {
			when {
				expression {params.test == true }
            }
            steps {
                sh 'echo "pwetpwet"'
            }
		}
	}
}

