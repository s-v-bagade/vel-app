pipeline {

	agent {

				label {

						label "node1"
					    customWorkspace "/mnt/project"
				}	
	}

	stages {
		stage ("test") {

					steps {
                        sh "sudo chmod -R 777 /mnt"
						echo "hello from node1"
					}
			}
		
		}

}
