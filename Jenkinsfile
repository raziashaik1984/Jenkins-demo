pipeline{

	agent any

	environment {
		DOCKERHUB_CREDENTIALS=credentials('dockerhub')
	}

	stages {
	    
	    stage('gitclone') {

			steps {
				echo 'Clone Process started'
				git 'https://github.com/raziashaik1984/Jenkins-demo.git'
				echo 'Clone Process end'
			}
		}

		stage('Build') {

			steps {
				echo 'Build Process started'
				sh 'docker build -t raziashaik1984/nodeapp_test:latest C:\ProgramData\Jenkins\.jenkins\workspace\node.js'
				echo 'Build Process end'
			}
		}

	}



}
