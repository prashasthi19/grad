pipeline{
	agent any
	tools{
		gradle 'gradle'
		jdk 'jdk'
	}
	stages{
		stage('Checkout'){
			steps{
				git branch:'master', url:'https://github.com/prashasthi19/grad.git'
			}
		}
		stage('Build'){
			steps{
				sh 'gradle build'
			}
		}
		stage('Test'){
			steps{
				sh 'gradle test'
			}
		}
		stage('Run Application'){
			steps{
				sh 'gradle hello'
			}
		}
	}
}

