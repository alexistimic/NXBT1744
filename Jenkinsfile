properties([
    [$class: 'BuildDiscarderProperty', strategy: [$class: 'LogRotator', daysToKeepStr: '60', numToKeepStr: '30', artifactNumToKeepStr: '1']],
    disableConcurrentBuilds(),
    [$class: 'GithubProjectProperty', displayName: '', projectUrlStr: 'https://github.com/nuxeo/'],
    [$class: 'RebuildSettings', autoRebuild: false, rebuildDisabled: false],
    [$class: 'ParametersDefinitionProperty', parameterDefinitions: [
        [$class: 'StringParameterDefinition', defaultValue: 'master', description: '', name: 'BRANCH'],
        [$class: 'StringParameterDefinition', defaultValue: 'master', description: '', name: 'PARENT_BRANCH']]],
    pipelineTriggers([[$class: 'GitHubPushTrigger']])
  ])

node('master'){
	timestamps {
		   timeout(time: 240, unit: 'MINUTES') {

			if (![$class: 'BuildDiscarderProperty']) {
				mail bcc: '', body: 'Builddiscarder does not exists', cc: '', from: '', replyTo: '', subject: 'pipeline_discardbuild_test', to: 'atimic@nuxeo.com'
			}
			else {
			mail bcc: '', body: 'builddiscarder exists', cc: '', from: '', replyTo: '', subject: 'pipeline_discardbuild_test', to: 'atimic@nuxeo.com'
			}
			echo "Hello world"
			}
		}
}
