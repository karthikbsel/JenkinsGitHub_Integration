pipeline {
					
					agent any
					
					tools {
						maven "Maven_Home"
					}
					stages {
						stage('Stage 1 - Checkout Code') {
							steps {
								//Get the code form GITHUB							
                                git 'https://github.com/ajautomation/PassParametersRunTimeViaMVN'
							}
						}
						stage('Stage 2 - Compile Code') {
							steps {
								//cmd to compile the code							
                                bat "mvn compile"
                                //sh "mvn compile"
							}
						}
						stage('Stage 3 - Run Unit Tests') {
							steps {
								//cmd to run tests							
                                bat "mvn test"
							}
						}
					}	
				}
