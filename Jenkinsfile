pipeline {
	agent any
		stages {
			stage('One') {
				steps {
					sh 'echo "Setting environment variable to true"'
                    env.EXECUTE='True'
				}
			}

			stage('Two') {
				when {
                    environment name: 'EXECUTE', value:'True'
                }
                steps {
					sh 'echo "Updating Second Stage, environment variable value:"'
                    sh 'echo ${EXECUTE}'
				}
			} 

			stage('Three') {
                when {
                    environment name: 'EXECUTE', value:'False'
                }
				steps {
					sh 'echo "Executing third stage because the value of the environment variable is: ${EXECUTE}"'
				}
			}
		}
}
