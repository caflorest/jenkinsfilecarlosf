pipeline {
	agent any
	    environment {
        	EXECUTE = "true"
	    }
		    stages {
			    stage('First') {
				    steps {
				        echo "${EXECUTE}"
				        sh '''
					    echo "Step one"
				    	'''
				     }
			     }

			    stage('Second') {
			        when {
				       environment name: "EXECUTE" , value: "true"
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
