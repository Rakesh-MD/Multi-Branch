pipeline {
    agent any

    stages {
        stage('Parallel Stages') {
            parallel {
                // Stage 1: Build
                build: {
                    steps {
                        echo 'Building...'
			sh 'sleep 30'
                        // Your build steps go here
                    }
                }

                // Stage 2: Test
                test: {
                    steps {
                        echo 'Testing...'
                        sh 'sleep 30'
			// Your test steps go here
                    }
                }
            }
        }

        // Additional stages after parallel execution
        stage('Deploy') {
            steps {
                echo 'Deploying...'
		sh 'sleep 30'
                // Your deployment steps go here
            }
        }
    }
}

