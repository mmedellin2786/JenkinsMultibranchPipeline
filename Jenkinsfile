pipeline {
        agent any
                stages {
                        stage('First') {
                                steps {
								        sh 'EXECUTE=True'
										sh 'echo $EXECUTE'
                                }
                        }


                        stage('Second') {
                                steps {
                                        sh 'echo "Updating second stage"'
                                }
                        }

                        stage('Third') {
                                steps {
                                        sh 'echo "Step Three"'
                                }
                        }
                }
}
