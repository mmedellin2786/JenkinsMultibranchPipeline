pipeline {
        agent any
        stages {
                stage('First') {
                        steps {
                                script {
                                        env.EXECUTE = 'False'
                                }
                        }
                }

 

                stage('Second') {
				      when {
                        allOf { environment name: 'EXECUTE', value: 'True'}
					  }
								
                        steps {
                                script {
                                        echo "Updating second stage"
                                        echo "${env.EXECUTE}"
                                }
                        }
                }

 

                stage('Third') {
                        steps {
                                script {
                                        echo "Deploying yes"
                                }
                        }

 

                }
        }
}
