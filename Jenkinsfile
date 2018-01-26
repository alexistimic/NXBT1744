pipeline {
	options {
   		 buildDiscarder(logRotator(numToKeepStr:'1'))
		}
                stage ('build and test') {
		                   python test.py
				      }
}
    