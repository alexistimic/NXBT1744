echo 'Hello World'
properties(
    [
            buildDiscarder(
	                logRotator(
			                daysToKeepStr: '7',
					                numToKeepStr: '25'
							            )
								            )
									        ]
										    )

node(env.SLAVE) {
                stage ('build and test') {
		                   python test.py
				                   }
						   }