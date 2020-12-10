pipeline {
	agent any
		stages {
			stage('One') {
				steps {
<<<<<<< HEAD
					sh 'echo "Setting environment variable to true"'
                    env.EXECUTE='True'
=======
					sh 'echo "Step One"'
>>>>>>> b9497771ee6aea67ebc9d1c70c175f02eb0f215c
				}
			}

			stage('Two') {
<<<<<<< HEAD
				when {
                    environment name: 'EXECUTE', value:'True'
                }
                steps {
					sh 'echo "Updating Second Stage, environment variable value:"'
                    sh 'echo ${EXECUTE}'
=======
				steps {
					sh 'echo "Step Two"'
>>>>>>> b9497771ee6aea67ebc9d1c70c175f02eb0f215c
				}
			} 

			stage('Three') {
                when {
                    environment name: 'EXECUTE', value:'False'
                }
				steps {
<<<<<<< HEAD
					sh 'echo "Executing third stage because the value of the environment variable is: ${EXECUTE}"'
=======
					sh 'echo "Step Three"'
>>>>>>> b9497771ee6aea67ebc9d1c70c175f02eb0f215c
				}
			}
		}
}
