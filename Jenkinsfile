pipeline{

	agent any

	environment {
		DOCKERHUB_CREDENTIALS=credentials('dockerhub')
	}

	stages {
	    
	    stage('gitclone') {

			steps {
				echo 'clone process started'
				git 'https://github.com/raziashaik1984/Jenkins-demo.git'
				echo 'clone process end'
			}
		}


	}

}
