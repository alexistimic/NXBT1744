node(env.SLAVE) {
                stage ('build and test') {
		                   python test.py
				                   }
						   }

options {
    buildDiscarder(logRotator(numToKeepStr:'1'))
    }