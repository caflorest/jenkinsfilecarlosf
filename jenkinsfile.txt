
	#este es un pipeline para el challenge devops dec16
	
pipeline {
	agent any
		stages {
			stage('One') {
				steps {
					sh '
						echo "Step One"
					'
				}
			}


			stage('Two') {
				steps {
					sh '
						echo "Step Two"
					'
				}
			} 

			stage('Three') {
				steps {
					sh '
						echo "Step Three"
					'
				}
			}
		}
}

