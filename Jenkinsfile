node('master') {
    configure { project ->
            // Doesn't take into account existing node
	            project << logRotator {
		                daysToKeep(-1)
				            numToKeep(10)
					                artifactDaysToKeep(-1)
							            artifactNumToKeep(-1)
								            }

        // Alters existing value
	       //(project / logRotator / daysToKeep).value = 2
		   }
}