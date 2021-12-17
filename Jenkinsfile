pipeline {
	agent any
	    environment {
        	execute = "true"
   	    
		    stages {
			    stage('First') {
				    steps {
				        echo "${execute}"
				        sh '''
					    echo "Step one"
				    	'''
				     }
			     }

			    stage('Second') {
			        when {
				       environment name: "execute" , value: "true"
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
}	
