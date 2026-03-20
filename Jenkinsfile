pipeline {

	agent {

				label {

						label "node1"
						customWorkspace "/mnt/project"
				}	
	}

	stages {

			stage ("install httpd") {

					steps {

							sh "sudo yum install httpd -y"
						}
			}

		stage ("start httpd") {

					steps {

							sh "sudo service httpd start"
						}
			}

		stage ("deploy index") {

					steps {

							sh "sudo cp -r index.html /var/www/html/"
							sh "sudo chmod -R 777 /var/www/html/index.html"
						}
			}
		
		}

}
