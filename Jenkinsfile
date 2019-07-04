pipeline {
        agent any
        stages {
                stage('First') {
                        steps {
                                script {
                                        env.EXECUTE = 'True'
                                }
                        }
                }

 

                stage('Second') {
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
