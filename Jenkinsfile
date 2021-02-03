pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh'''
                mvn clean compile
		echo "Compile"
                '''
                }
            }
        stage('Test'){
            steps {
                sh'''
                mvn clean test
                '''
            }
        }
        stage('Deploy') {
            steps {
                sh'''
                mvn clean package
                '''

            }
        }
    }
	}
