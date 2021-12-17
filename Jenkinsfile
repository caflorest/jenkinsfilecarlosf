pipeline {
	agent any
		stages {
			stage('First') {
				steps {
					script {
						env.execute = true
					}
					echo "${env.execute}"
					sh '''
						echo "Step one"
					'''
				}
			}

			stage('Second') {
			when {
				expression {
					env.execute == true
				}

				steps {
					sh '''
						echo "Updating Second Stage"
					'''
				}
			}

			stage('Third') {
				steps {
					sh '''
						echo "Step Three"
					'''
				}
			}
		}
}
