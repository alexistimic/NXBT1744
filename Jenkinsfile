node('master'){
	properties([[$class: 'BuildDiscarderProperty',
		     strategy: [$class: 'LogRotator', artifactDaysToKeepStr: '',
		     artifactNumToKeepStr: '1',
		     daysToKeepStr: '60',
		     numToKeepStr: '60']]])
		}