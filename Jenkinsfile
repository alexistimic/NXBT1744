properties([[$class: 'BuildDiscarderProperty',
		     strategy: [$class: 'LogRotator', artifactDaysToKeepStr: '',
		     artifactNumToKeepStr: '1',
		     daysToKeepStr: '60',
		     numToKeepStr: '60']]])

node('master'){
	timestamps {
		   timeout(time: 240, unit: 'SECONDS') {
		   python test.py	   
			}
		}
}